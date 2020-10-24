'''
<?php
show_source("index1.php");
include "flag.php";
if(isset($_GET['a']) and isset($_GET['b'])){
    if($_GET['a']==$_GET['b']){
        echo 'a and b must be different';
    }
    else if (sha1($_GET['a'])===sha1($_GET['b'])){
        echo "$flag";
    }
    else{
     echo 'more thinking';
    }
}
?>
'''
