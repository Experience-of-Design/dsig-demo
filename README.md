# Uk�zkov� aplikace pro podepisov�n� a p�id�n� �asov�ho raz�tka do dokument� ISDOC

## Po�adavky

Uk�zkov� aplikace je napsan� v jazyce C# pro prost�ed� .NET. Sou��st� je i projekt pro Visual
Studio 2013, kter� dovoluje snadn� spou�t�n� aplikace. Visual Studio je mo�n� z�skat ve verzi Exprss zdarma
na adrese http://www.visualstudio.com/en-us/products/visual-studio-express-vs.aspx

### Vygenerov�n� testovac�ch certifik�t�

Aplikace pro podepisov�n� pou��v� testovac� certifik�ty. Ty je mo�n� vygenerovat pomoc� p��kazu `makecert`.
P��kaz je dostupn� po spu�t�n� **Visual Studio Command Prompt**.

````
makecert -r -pe -n "CN=Jan Nov�k" -ss My
makecert -r -pe -n "CN=Jana Proch�zkov�" -ss My
````

Certifik�ty si m��ete vygenerovat v��e uveden�m postupem znovu, nebo je m��ete importovat. Sta��
otev��t soubory `novak.pfx` a `prochazkova.pfx` ulo�en� v adres��i `data`. Prost�ed� Windows automaticky
zp�st� pr�vodce importem certifik�tu.

### Spr�vce certifik�t�

P�i pr�ci s digit�ln�mi podpisy v prost�ed� Windows je u�ite�n� pou��vat spr�vce certifik�t�. Ten lze spustit pomoc� **Start -> Spustit -> 
certmgr.msc**

Osobn� certifik�ty je mo�n� spravovat na z�lo�ce **Personal -> Cetificates** (Osobn� -> Certifik�ty).



