[Page Source Code](https://github.com/CSC109/MarkdownWebsite/blob/master/code-blocks.md){:target="_blank"}

[Home](./)

# Code Blocks

## Without Syntax Highlighting

`One line`

```
multiple
lines
```

## With Syntax Highlighting

Full list of supported languages [here](https://www.rubycoloredglasses.com/2013/04/languages-supported-by-github-flavored-markdown/).

### Java

```java
public static void main(String[] args) {
    String message = "Hello world";
    System.out.println(message);
}
```

### Scala

```scala
val message = "Hello world"
println(message)
```

### Python

```python
message = 'Hello world'
print(message)
```

### JavaScript

```javascript
const message = 'Hello world'
console.log(message)
```

### HTML

```html
<div>
    <p>Hello world</p>
</div>
```

### JSON

```json
{
    "message": "Hello world"
}
```

### C#

```csharp
public static void main(string[] args) {
    string message = "Hello world";
    Console.WriteLine(message);
}
```