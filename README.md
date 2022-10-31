# anchors-test
Check case-sensetivity and other conversion rules of GitHub anchors

`a.md` has headings `H1`, `Some heading`, `Heading with dot.`, `Heading with dot. And some words after`

- `a.md#h1` [working](a.md#h1)
- `a.md#H1` [working](a.md#H1)
- `a.md#SoMe-HeAdInG` [working](a.md#SoMe-HeAdInG)
- `a.md#someheading` [broken](a.md#someheading)
- `a.md#Heading-with-dot` [working](a.md#Heading-with-dot)
- `a.md#heading-with-dot-` [broken](a.md#heading-with-dot-)
- `a.md#heading-with-dot-and-some-words-after` [working](a.md#heading-with-dot-and-some-words-after)
- `a.md#heading-with-dot--and-some-words-after` [broken](a.md#heading-with-dot--and-some-words-after)
