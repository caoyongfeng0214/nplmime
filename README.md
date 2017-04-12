# npl-mime

## 示例

    local mime = NPL.load('mime');
    
    local mimeType = mime.get('html');
    print(mimeType);  -- text/html
    
    local mimeType2 = mime.get('abc');
    print(mimeType2);  -- application/octet-stream
    
    mime.set('abc', 'text/plain');
    local mimeType3 = mime.get('abc');
    print(mimeType3); -- text/plain
    
    local bl = mime.isPlainTextType('css');
    print(bl); -- true
    
    local bl2 = mime.isPlainTextType('exe');
    print(bl2); -- false
