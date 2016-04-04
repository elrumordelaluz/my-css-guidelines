# my-css-guidelines 
Some things useful to follow when write or start writint css (or scss).

### General things
- Keep the code readable
- It's a good idea to use an [.editorconfig](http://editorconfig.org/) file 
- The entire code-base should be based on the same _Style guide_

### Syntax and Format
- Use two (2) spaces indent
- Use one (1) space before `{` when declaring rules
- Selectors listed, each one in a new line
- Use one (1) space after `:` when declaring a property
- Write each rule per line
- Closing `}` better in a new line
- Use lowercase and (when possible) shorthand hex values (like `#3ac`)
- Use consistently single quotes (like `content: '\e601'`)
- Do not specify units on zerp-based values (like `padding: 0;`)
- One empty line between related rulesets
- Two empty lines between less related rulesets 
- Four or more empty lines between non related rulesets (see "Comments/Headings")
- Declare properties in alphabetical ordering.
- Use single-line format for big blocks of similar rulesets with only one declaration each
- Improve readability for long comma-separated property values (like gradients, shadows)

```css
.selector,
.another-selector {
  property: value;
  another-property: value;
}

.sel-1 { margin-top: 1rem; }
.sel-2 { margin-top: 2rem; }
.sel-3 { margin-top: 3rem; }

.sel-shadow {
  box-shadow:
    1px 0 1px #aaa,
    2px 0 2px #ccc;
}
```

### Comments and Headings
- Open each _performant_ module section with a good description of it: how it works, benefits and limitations
- Keep the line-length to 80 columns

```scss
/// -------------------------------------------------------------------------
///  This is a New Section
/// -------------------------------------------------------------------------

///  This is a sub Section
/// -------------------------------------------------------------------------

/// -
/// This is a Description
///
/// Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam 
/// repellendus quidem iste veritatis et officia eum laboriosam neque qui.
///
/// @info
///
/// TODO: Necessitatibus id, perspiciatis eos quod, deserunt nostrum facilis 
///   pariatur quasi debitis harum ex modi,
/// -

/// Simple comment
```

### Other little things
- Remove (automatic or manually) the last end-of-line whitespace



