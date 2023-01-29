
## SetOption and Executing Measure/Plugin function

```
[sWebParser]
Measure=WebParser
URL=

[Box]
Meter=Image
W=80
H=80
LeftMouseUpAction=[!CommandMeasure sWebParser "Update"][!SetOption sWebParser URL "https://example.com/"][!UpdateMeasure sWebParser]
```

<p><br></p?

**[WebParser](https://docs.rainmeter.net/manual/measures/webparser/)** measure

```
[!CommandMeasure sWebParser "Update"][!SetOption sWebParser URL "https://example.com/"][!UpdateMeasure sWebParser]
```
or
```
[!SetOption sWebParser URL "https://example.com/"][!CommandMeasure sWebParser "Update"][!UpdateMeasure sWebParser]
```


**[RunCommand](https://docs.rainmeter.net/manual/plugins/runcommand/)** plugin
```
[!SetOption sRunCommand Parameter "dir /b"][!UpdateMeasure sRunCommand][!CommandMeasure sRunCommand "Run"]
```
