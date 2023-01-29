
## SetOption and Executing Measure/Plugin function

```
[sWebParser]
Measure=WebParser
URL=

[Box]
Meter=Image
W=80
H=80
LeftMouseUpAction=[!SetOption sWebParser URL "https://example.com/"][!CommandMeasure sWebParser "Update"][!UpdateMeasure sWebParser]
```

<p><br></p?

**[WebParser](https://docs.rainmeter.net/manual/measures/webparser/)** measure
```
[!SetOption sWebParser URL "https://example.com/"][!CommandMeasure sWebParser "Update"][!UpdateMeasure sWebParser]
```


**[RunCommand](https://docs.rainmeter.net/manual/plugins/runcommand/)** plugin
```
[!SetOption sRunCommand Parameter "dir /b"][!UpdateMeasure sRunCommand][!CommandMeasure sRunCommand "Run"]
```
