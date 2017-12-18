# Travis

**Ci�g�a integracja** to praktyka tworzenia oprogramowania, polegaj�ca na cz�stej integracji kodu, zazwyczaj pochodz�cego od r�znych programist�w. 
Opr�cz integracji nale�y zapewnieni� tak�e poprawno�� kompilacji kodu �r�d�owego.
Dlatego do naszego kodu powinni�my mie� napisane odpowiednie testy, kt�re sprawdz� jego poprawno��. 

Korzy�ci z automatycznego uruchamiania test�w:
- nie trzeba pami�ta� o uruchamianiu test�w,
- w wypadku wykrycia b��du automatycznie wszyscy zainteresowaniu mog� dosta� stosowne powiadomienie,
- dost�pna jest historia przebiegu test�w kolejnych wersji kodu,
- zwi�ksza poziom zaufania do pakietu.

[**Travis CI**](https://travis-ci.org/) - narz�dzie wspomagaj�ce ci�g�� integracj� projekt�w znajduj�cych si� na GitHubie.

[Getting started](https://docs.travis-ci.com/user/getting-started/)

[Building na R Project](https://docs.travis-ci.com/user/languages/r/)

[Building a Python Project](https://docs.travis-ci.com/user/languages/python/)

[Checking after every commit with Travis by Hadley Wickham](http://r-pkgs.had.co.nz/check.html#travis)

## Konfiguracja

Travisa konfiguruje si� poprzez plik .travis.yml umieszczony w repozytorium projektu. 
Przyk�adowa zawarto�� [pliku konfiguracyjnego](https://github.com/mi2-warsaw/MI2DataLab_Seminarium/blob/master/2017_12_19_travis/.travis.yml):

```
language: R
sudo: false
cache: packages

notifications:
  email: false
```

Inne przydatne opcje:

`r_github_packages` - instalacja pakiet�w z GitHuba

`r_binary_packages` - instalowanie prekompilowanych pakiet�w. Ta opcja pozwala zredukowa� czas budowy Travisa. 
List� dost�pnych pakiet�w mo�na znale�� na [stronie z pakietami dla systemu Ubuntu](https://packages.ubuntu.com/)



# AppVeyor

[AppVeyor](https://www.appveyor.com/) -  ci�g�a integracja - budowanie i testowanie projekt�w hostowanych na GitHubie na wirtualnej maszynie z Microsoft Windows.

[Jak u�ywa� AppVeyor w projektach R.](https://github.com/krlmlr/r-appveyor)