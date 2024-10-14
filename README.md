- Install pandoc in local system
- Install xelatex pdf engine in your local system

- install necessary tex packages like (enumitem,lastpage,sectsty).
- replace markdown content in example.md file
- run below command in your terminal (change variable value as per your content)

```
pandoc example.md -o output.pdf \
  --template=custom.latex \
  --pdf-engine=xelatex \
  -V smallHeader="fraction addition" \
  -V concept="fraction addition" \
  -V grade="Grade 6" \
  -V additionalCriteria="-" \
  -V totalTime="80 minutes"
```
