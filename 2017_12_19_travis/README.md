# Travis - continuous integration

*Ci�g�a* integracja to praktyka tworzenia oprogramowania, polegaj�ca na cz�stej integracji kodu, zazwyczaj pochodz�cego od r�znych programist�w. 

[*Travis CI*](https://travis-ci.org/) - narz�dzie wspomagaj�ce ci�g�� integracj� projekt�w znajduj�cych si� na GitHubie.

[Travis CI, przyjemne Continuous Integration dla projekt�w na GitHubie](http://www.simplecoding.pl/travis-ci/)

[Getting started](https://docs.travis-ci.com/user/getting-started/)

[Building na R project](https://docs.travis-ci.com/user/languages/r/)


## Konfiguracja

Travisa konfiguruje si� poprzez plik .travis.yml umieszczony w repozytorium projektu. 
Przyk�adowa zawarto�� pliku konfiguracyjnego:

```
language: R
sudo: false
cache: packages

notifications:
  email: false
```



