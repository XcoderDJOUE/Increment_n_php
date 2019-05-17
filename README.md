# Increment_n_php
function permetant de faire les incrementation du genre numero de bon ou id  en php simple et pratique


function increment_n($taille_maxi=9999, $numpreceent = 0){
$preced = $numpreceent;
$taille=$taille_maxi;
if(strlen(strval($preced)) > strlen($taille)){
   $taille = $taille + intval(1 . strlen(strval($preced))); 
}
$re = $taille + $preced;
$retour = $re - $taille;
$va_f = "";
$nbrzero=0;
$sero = 0;
for($i=0 ; $i < strlen($taille); $i++){
    $sero = strlen($preced);
    $nbrzero = strlen($taille) -  $sero;
}
for($h=0; $h < $nbrzero; $h++){
  $va_f .= 0;  
}
$va_f .= $preced+1;
return $va_f;
}




**************************initialisation de la function **********************************

increment_n(9999, 0);


*****parametre

*parametre 1 : sert de masque de debut de comptage . si vous voullez commencé a compter a 0001 alors metter 9999 et si ces 00001 alors ces 99999 ainsi de suite ...

*parametre 2 : increment en fonction du numero precent de l'ecmenttation entré ici . si vous entré 100 avec comme param 1 : 9999 alors il incrementera a 0101
