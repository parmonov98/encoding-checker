# encoding-checker

```
function encoding_checker($string){
    $arr = [];
    foreach(mb_list_encodings() as $chr){
        $arr[] = mb_convert_encoding($string, 'UTF-8', $chr)." : ".$chr."<br>";   
    }
    return $arr;
}
```
