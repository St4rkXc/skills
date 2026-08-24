# Docblock Standards Reference

Complete documentation standard specifications per language. Follow these exactly when generating inline docblocks.

---

## JavaScript (JSDoc)

Standard: [JSDoc](https://jsdoc.app/)

### Format

```javascript
/**
 * Calculates the total price including tax and discounts.
 *
 * Iterates through cart items, applies individual discounts,
 * then sums with the applicable tax rate.
 *
 * @param {CartItem[]} items - Array of cart items to calculate.
 * @param {number} taxRate - Tax rate as a decimal (e.g., 0.08 for 8%).
 * @param {Object} [options] - Optional calculation settings.
 * @param {boolean} [options.roundUp=false] - Whether to round up fractional cents.
 * @returns {number} The total price in the smallest currency unit (cents).
 * @throws {RangeError} If taxRate is negative or greater than 1.
 * @throws {TypeError} If items is not an array.
 *
 * @example
 * const items = [{ id: 1, price: 1000, qty: 2, discount: 0.1 }];
 * const total = calculateTotal(items, 0.08);
 * // => 1944
 *
 * @see CartItem
 * @since 2.0.0
 * @deprecated Use calculateTotalV2 instead.
 */
function calculateTotal(items, taxRate, options = {}) {
  // ...
}
```

### Required tags per entity type

| Entity | Required Tags |
|--------|--------------|
| Function/Method | `@param`, `@returns`, `@throws` (if throws) |
| Class | Description, `@example` |
| Interface/Type | Description of each property |
| Module | `@module` tag at file top |
| Constant | `@type`, description |
| Event | `@event`, `@fires` |

### Rules

- Use `@param {Type} name - Description` format (with hyphen separator)
- Optional params use `[name]` or `[name=default]`
- Destructured params: `@param {Type} options.key - Description`
- Union types: `@param {string|number} id`
- Nullable: `@param {?string} name` or `@param {string|null} name`
- Variadic: `@param {...string} names`

---

## TypeScript (TSDoc)

Standard: [TSDoc](https://tsdoc.org/)

### Format

```typescript
/**
 * Fetches a user by ID from the database.
 *
 * @param id - The unique identifier of the user.
 * @param options - Query options.
 * @param options.includeDeleted - Whether to include soft-deleted users.
 * @returns The user object if found.
 * @throws {NotFoundError} If no user exists with the given ID.
 *
 * @example
 * ```ts
 * const user = await getUser("usr_123", { includeDeleted: false });
 * ```
 *
 * @see createUser
 * @see updateUser
 */
export async function getUser(
  id: string,
  options: GetUserOptions = {}
): Promise<User> {
  // ...
}
```

### TSDoc-specific tags

| Tag | Purpose |
|-----|---------|
| `@typeParam` | Generic type parameter documentation |
| `@defaultValue` | Default value for optional params |
| `@override` | Indicates method overrides parent |
| `@sealed` | Prevents further overriding |
| `@beta` / `@alpha` | API stability markers |
| `@public` / `@internal` | Visibility markers |
| `@inheritDoc` | Inherit docs from another member |
| `@link` | Inline link to another API member |
| `@remarks` | Extended details beyond summary |
| `@decorator` | Documents a decorator |

### Rules

- Summary line must be a single sentence ending with period
- Use `@remarks` for extended description beyond the summary
- Use `@link` for cross-references: `{@link ClassName.methodName}`
- Code blocks must specify language: ` ```ts `
- `@typeParam T - The type of item in the collection`

---

## PHP (phpDoc / PSR-5 / PSR-19)

Standard: [PSR-5 (phpDocumentor)](https://docs.phpdoc.org/3.0/guide/references/phpdoc/index.html), [PSR-19](https://www.php-fig.org/psr/psr-19/)

### Format

```php
<?php

/**
 * Calculates the total price including tax and discounts.
 *
 * Iterates through cart items, applies individual discounts,
 * then sums with the applicable tax rate.
 *
 * @param CartItem[] $items    Array of cart items to calculate.
 * @param float      $taxRate  Tax rate as decimal (e.g., 0.08 for 8%).
 * @param array{roundUp?: bool} $options Optional settings.
 *
 * @return int Total price in smallest currency unit (cents).
 *
 * @throws RangeException If taxRate is negative or greater than 1.
 * @throws InvalidArgumentException If items is empty.
 *
 * @example
 *     $items = [new CartItem(id: 1, price: 1000, qty: 2, discount: 0.1)];
 *     $total = calculateTotal($items, 0.08);
 *     // => 1944
 *
 * @see CartItem
 *
 * @since 2.0.0
 * @deprecated Use calculateTotalV2() instead.
 */
function calculateTotal(array $items, float $taxRate, array $options = []): int
{
    // ...
}
```

### PSR-5/PSR-19 specific rules

- `@return` not `@returns` (PHP convention)
- Type alignment: align types and variable names with spaces
- Array shapes: `array{key: type, key2: type}`
- Generics: `Collection<int, User>`
- `@phpstan-*` and `@psalm-*` tags for static analysis types when needed
- `@inheritDoc` for inheriting parent docs
- `@mixin` for magic method delegation
- `@pure` / `@impure` for functional purity markers

### Required tags per entity

| Entity | Required Tags |
|--------|--------------|
| Function/Method | `@param`, `@return`, `@throws` (if throws) |
| Class | Description, `@property`, `@method` (for magic) |
| Interface | Description, method signatures documented |
| Trait | Description, usage context |
| Property | `@var` with type |
| Constant | `@var` with type, description |

---

## Python (PEP 257 / Google Style)

Standard: [PEP 257](https://peps.python.org/pep-0257/), [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings)

### Format

```python
def calculate_total(
    items: list[CartItem],
    tax_rate: float,
    *,
    round_up: bool = False,
) -> int:
    """Calculate the total price including tax and discounts.

    Iterates through cart items, applies individual discounts,
    then sums with the applicable tax rate.

    Args:
        items: Array of cart items to calculate.
        tax_rate: Tax rate as a decimal (e.g., 0.08 for 8%).
        round_up: Whether to round up fractional cents.
            Defaults to False.

    Returns:
        Total price in smallest currency unit (cents).

    Raises:
        ValueError: If tax_rate is negative or greater than 1.
        TypeError: If items is not a list.

    Examples:
        >>> items = [CartItem(id=1, price=1000, qty=2, discount=0.1)]
        >>> calculate_total(items, 0.08)
        1944

    Note:
        This function does not persist results. Use
        :meth:`Cart.save_total` for persistence.

    See Also:
        CartItem: The item data structure.
        calculate_total_v2: Updated version with caching.

    .. deprecated:: 2.0.0
        Use :func:`calculate_total_v2` instead.
    """
    ...
```

### Rules

- Module-level docstring at top of every `.py` file
- Class docstring after class definition, before `__init__`
- `__init__` documented in class docstring, not separately
- Use type hints in signature, not in docstring (Google style)
- One-liner docstrings for trivial functions: `"""Return the name."""` (period, imperative)
- Multi-line: summary line, blank line, then sections
- Section headers: `Args:`, `Returns:`, `Raises:`, `Examples:`, `Note:`, `Warning:`, `See Also:`, `Attributes:`, `References:`
- Doctest-compatible examples in `Examples:` section

---

## Java (Javadoc)

Standard: [Javadoc](https://docs.oracle.com/en/java/javase/17/docs/specs/doc-comment-spec.html)

### Format

```java
/**
 * Calculates the total price including tax and discounts.
 *
 * <p>Iterates through cart items, applies individual discounts,
 * then sums with the applicable tax rate. This method is thread-safe
 * and does not modify the input list.
 *
 * @param items    the list of cart items to calculate; must not be null or empty
 * @param taxRate  the tax rate as a decimal (e.g., 0.08 for 8%); must be 0.0-1.0
 * @param roundUp  whether to round up fractional cents
 * @return the total price in the smallest currency unit (cents)
 * @throws IllegalArgumentException if {@code taxRate} is negative or greater than 1
 * @throws NullPointerException     if {@code items} is null
 *
 * @example
 * <pre>{@code
 * List<CartItem> items = List.of(new CartItem(1, 1000, 2, 0.1));
 * int total = calculateTotal(items, 0.08, false);
 * // => 1944
 * }</pre>
 *
 * @see CartItem
 * @see #calculateTotalV2(List, double, boolean)
 * @since 2.0.0
 * @deprecated Use {@link #calculateTotalV2} instead.
 */
public int calculateTotal(List<CartItem> items, double taxRate, boolean roundUp) {
    // ...
}
```

### Rules

- First sentence = summary (terminated by period followed by space/tab/newline)
- Use `{@code ...}` for inline code, `{@link ...}` for cross-references
- Use `<pre>{@code ... }</pre>` for code blocks
- Use `{@inheritDoc}` to inherit from parent
- `@param`, `@return`, `@throws` required for all public methods
- `@serial` for serializable fields
- `@since` for version tracking
- HTML allowed in descriptions but keep minimal

---

## Go (godoc)

Standard: [Go Doc Comments](https://go.dev/doc/comment)

### Format

```go
// CalculateTotal calculates the total price including tax and discounts.
//
// It iterates through cart items, applies individual discounts,
// then sums with the applicable tax rate.
//
// Parameters:
//   - items: slice of cart items to calculate. Must not be empty.
//   - taxRate: tax rate as decimal (e.g., 0.08 for 8%). Must be 0.0-1.0.
//   - opts: optional calculation settings.
//
// Returns the total price in the smallest currency unit (cents).
//
// Returns an error of type RangeError if taxRate is out of bounds,
// or TypeError if items is nil.
//
// Example:
//
//	items := []CartItem{{ID: 1, Price: 1000, Qty: 2, Discount: 0.1}}
//	total, err := CalculateTotal(items, 0.08, nil)
//	// total == 1944
//
// See also: CartItem, CalculateTotalV2.
func CalculateTotal(items []CartItem, taxRate float64, opts *Options) (int, error) {
	// ...
}
```

### Rules

- Comment directly above declaration, no blank line between
- Start with the name of the thing being described: `// CalculateTotal calculates...`
- Package-level doc in `doc.go` or at top of package file
- First sentence appears in godoc index — make it count
- Use `// Example:` blocks for runnable examples
- Exported names must have doc comments (lint enforced)
- Unexported names: comment only if non-obvious
- No markdown in godoc (plain text with indentation for code)
- Link to other identifiers by name: `See also: CartItem.`

---

## C# (XML Doc Comments)

Standard: [XML Doc Comments](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/xmldoc/)

### Format

```csharp
/// <summary>
/// Calculates the total price including tax and discounts.
/// </summary>
/// <remarks>
/// Iterates through cart items, applies individual discounts,
/// then sums with the applicable tax rate.
/// </remarks>
/// <param name="items">Array of cart items to calculate.</param>
/// <param name="taxRate">Tax rate as a decimal (e.g., 0.08 for 8%).</param>
/// <param name="options">Optional calculation settings.</param>
/// <returns>The total price in the smallest currency unit (cents).</returns>
/// <exception cref="ArgumentOutOfRangeException">
/// Thrown when <paramref name="taxRate"/> is negative or greater than 1.
/// </exception>
/// <exception cref="ArgumentNullException">
/// Thrown when <paramref name="items"/> is null.
/// </exception>
/// <example>
/// <code>
/// var items = new[] { new CartItem { Id = 1, Price = 1000, Qty = 2, Discount = 0.1m } };
/// var total = CalculateTotal(items, 0.08m);
/// // => 1944
/// </code>
/// </example>
/// <seealso cref="CartItem"/>
/// <seealso cref="CalculateTotalV2"/>
public int CalculateTotal(CartItem[] items, decimal taxRate, Options? options = null)
{
    // ...
}
```

### Rules

- `<summary>` required for all public members (compiler warning if missing)
- Use `<paramref name="x"/>` to reference parameters in text
- Use `<see cref="Member"/>` for cross-references
- Use `<code>` inside `<example>` for code blocks
- `<include file="" path=""/>` for external doc files
- `<inheritdoc/>` to inherit from base/interface
- `<value>` for property descriptions
- `<typeparam>` for generic type parameters
- `<returns>` required for non-void methods

---

## Rust (rustdoc)

Standard: [rustdoc](https://doc.rust-lang.org/rustdoc/)

### Format

```rust
/// Calculates the total price including tax and discounts.
///
/// Iterates through cart items, applies individual discounts,
/// then sums with the applicable tax rate.
///
/// # Arguments
///
/// * `items` - Slice of cart items to calculate. Must not be empty.
/// * `tax_rate` - Tax rate as a decimal (e.g., 0.08 for 8%).
/// * `options` - Optional calculation settings.
///
/// # Returns
///
/// The total price in the smallest currency unit (cents).
///
/// # Errors
///
/// Returns [`CalcError::InvalidTaxRate`] if `tax_rate` is out of bounds.
/// Returns [`CalcError::EmptyItems`] if `items` is empty.
///
/// # Panics
///
/// Panics if any item has a negative price.
///
/// # Examples
///
/// ```
/// use mylib::calculate_total;
///
/// let items = vec![CartItem { id: 1, price: 1000, qty: 2, discount: 0.1 }];
/// let total = calculate_total(&items, 0.08, None).unwrap();
/// assert_eq!(total, 1944);
/// ```
///
/// # See also
///
/// - [`CartItem`] for the item data structure.
/// - [`calculate_total_v2`] for the cached version.
pub fn calculate_total(
    items: &[CartItem],
    tax_rate: f64,
    options: Option<Options>,
) -> Result<i64, CalcError> {
    // ...
}
```

### Rules

- `///` for item-level docs, `//!` for module-level docs
- Section headers: `# Arguments`, `# Returns`, `# Errors`, `# Panics`, `# Examples`, `# Safety` (for unsafe), `# See also`
- Examples must be runnable doctests (compiled and tested by `cargo test`)
- Use `[`Type`]` for intra-doc links
- `# Safety` section required for `unsafe fn`
- Module docs at top of `lib.rs` or `mod.rs` with `//!`

---

## Ruby (YARD)

Standard: [YARD](https://rubydoc.info/gems/yard/file/docs/Tags.md)

### Format

```ruby
# Calculates the total price including tax and discounts.
#
# Iterates through cart items, applies individual discounts,
# then sums with the applicable tax rate.
#
# @param items [Array<CartItem>] array of cart items to calculate
# @param tax_rate [Float] tax rate as decimal (e.g., 0.08 for 8%)
# @param options [Hash] optional settings
# @option options [Boolean] :round_up (false) whether to round up fractional cents
# @return [Integer] total price in smallest currency unit (cents)
# @raise [RangeError] if tax_rate is negative or greater than 1
# @raise [TypeError] if items is not an array
#
# @example Calculate total for two items
#   items = [CartItem.new(id: 1, price: 1000, qty: 2, discount: 0.1)]
#   calculate_total(items, 0.08)
#   # => 1944
#
# @see CartItem
# @see #calculate_total_v2
# @since 2.0.0
# @deprecated Use {#calculate_total_v2} instead.
def calculate_total(items, tax_rate, **options)
  # ...
end
```

### Rules

- `@param name [Type] description` format
- `@return [Type] description` (not `@returns`)
- `@raise [ExceptionType] condition`
- `@option hash_name [Type] :key (default) description`
- `@overload` for methods with multiple signatures
- `@abstract` for abstract methods
- `@yield` and `@yieldparam` for blocks
- `@note`, `@todo`, `@deprecated` for metadata
- `@!attribute`, `@!method`, `@!visibility` for dynamic definitions

---

## Swift (Swift Markup)

Standard: [Swift Markup](https://developer.apple.com/library/archive/documentation/Xcode/Reference/xcode_markup_formatting_ref/)

### Format

```swift
/// Calculates the total price including tax and discounts.
///
/// Iterates through cart items, applies individual discounts,
/// then sums with the applicable tax rate.
///
/// - Parameters:
///   - items: Array of cart items to calculate.
///   - taxRate: Tax rate as a decimal (e.g., 0.08 for 8%).
///   - options: Optional calculation settings.
/// - Returns: The total price in the smallest currency unit (cents).
/// - Throws: `CalcError.invalidTaxRate` if `taxRate` is out of bounds.
///   `CalcError.emptyItems` if `items` is empty.
///
/// - Example:
///   ```swift
///   let items = [CartItem(id: 1, price: 1000, qty: 2, discount: 0.1)]
///   let total = try calculateTotal(items, taxRate: 0.08)
///   // => 1944
///   ```
///
/// - Remark: This function does not persist results.
/// - SeeAlso: `CartItem`, `calculateTotalV2(items:taxRate:options:)`
/// - Since: 2.0.0
/// - Deprecated: Use `calculateTotalV2` instead.
func calculateTotal(
    _ items: [CartItem],
    taxRate: Double,
    options: Options? = nil
) throws -> Int {
    // ...
}
```

### Rules

- `- parameter name:` or `- Parameters:` with nested `- name:` for multiple
- `- returns:`, `- throws:`, `- note:`, `- warning:`, `- important:`
- `- requires:` for preconditions
/// `- SeeAlso:` for cross-references (note: capitalization matters)
/// `- Example:` for code examples
/// `- Since:` for version tracking
/// Use `///` not `/** */` for Swift

---

## Kotlin (KDoc)

Standard: [KDoc](https://kotlinlang.org/docs/kotlin-doc.html)

### Format

```kotlin
/**
 * Calculates the total price including tax and discounts.
 *
 * Iterates through cart items, applies individual discounts,
 * then sums with the applicable tax rate.
 *
 * @param items list of cart items to calculate; must not be empty.
 * @param taxRate tax rate as a decimal (e.g., 0.08 for 8%).
 * @param options optional calculation settings.
 * @return the total price in the smallest currency unit (cents).
 * @throws IllegalArgumentException if `taxRate` is negative or greater than 1.
 * @throws IllegalStateException if `items` is empty.
 *
 * @sample com.example.CalculateTotalTest.basicCalculation
 *
 * @see CartItem
 * @see calculateTotalV2
 * @since 2.0.0
 * @deprecated Use [calculateTotalV2] instead.
 */
fun calculateTotal(
    items: List<CartItem>,
    taxRate: Double,
    options: Options? = null
): Int {
    // ...
}
```

### Rules

- `[ClassName]` for cross-references (auto-links)
- `@sample` to reference test examples
- `@property` for property descriptions in class docs
- `@constructor` for constructor documentation
- `@receiver` for extension function receiver
- `@suppress` to hide from generated docs
- No `@typeParam` — use description in class-level doc

---

## Dart (dartdoc)

Standard: [dartdoc](https://dart.dev/tools/dart-doc)

### Format

```dart
/// Calculates the total price including tax and discounts.
///
/// Iterates through cart items, applies individual discounts,
/// then sums with the applicable tax rate.
///
/// The [items] parameter must not be empty. The [taxRate] must be
/// between 0.0 and 1.0.
///
/// Returns the total price in the smallest currency unit (cents).
///
/// Throws a [RangeError] if [taxRate] is negative or greater than 1.
/// Throws an [ArgumentError] if [items] is empty.
///
/// Example:
/// ```dart
/// final items = [CartItem(id: 1, price: 1000, qty: 2, discount: 0.1)];
/// final total = calculateTotal(items, 0.08);
/// // => 1944
/// ```
///
/// See also:
/// * [CartItem], the item data structure.
/// * [calculateTotalV2], the cached version.
///
/// @deprecated Use [calculateTotalV2] instead.
int calculateTotal(List<CartItem> items, double taxRate, {bool roundUp = false}) {
  // ...
}
```

### Rules

- `[ClassName]` for cross-references (auto-links)
- Square brackets link to identifiers automatically
- `///` for item docs, `//!` not used (use library-level `///`)
- Code blocks with triple backticks and language tag
- `@deprecated`, `@override`, `@immutable`, `@proxy`, `@sealed`
- See also section as bullet list
