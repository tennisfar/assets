# Usage

Snippet:

```javascript
asset = document.getElementById('asset');

if (!asset) {
    ss = document.createElement('img');
    ss.id = 'asset';
    document.body.appendChild(ss);
}

assetStyle = document.getElementById('assetStyle');

if (!assetStyle) {
    style = document.createElement('style');
    style.id = 'assetStyle';
    document.body.appendChild(style);
}

style.innerHTML = `
#asset {
    position: fixed;
    top: 0;
    left: 0;
    pointer-events: none;
    opacity: 0.3;
}
`;

ss.src = 'http://localhost:60109/compliance-casino/ss.png';
```
