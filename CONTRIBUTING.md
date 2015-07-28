# Kontribuoni tek PHP Mënyra e saktë

Ju pëlqen [PHP The Right Way](http://phptherightway.com) dhe doni të 
përfshiheni në këtë projekt? Fantastike! Ka disa mënyra se si mund të ndihmoni.

Ju lutemi kushtojini një moment këtij dokumenti në mënyrë që të kryeni procesin 
e kontribuimit sa më lehtë dhe efektivisht për të gjithë që janë të përfshirë tek ky projekt.

Duke ndjekur këto këshilla tregoni që respektoni kohën që zhvilluesit kushtojnë 
për të menaxhuar dhe zhvilluar këtë projekt me burim të hapur. Në këmbim, do t'ju 
këmbehet reciprokisht respekti tek adresimi i problemeve tuaja ose marrja parasysh 
e patch-eve dhe funksionaliteteve të reja.

## Përdorimi i ndjekësit të problemeve

[Ndjekësi Problemeve](https://github.com/anooxy/php-the-right-way/issues) është 
kanali i preferuar per këto ndryshime: probleme gërmëzimi, ndryshime fjalësh, përmbajtje 
të re dhe [krijimin e pull requests](#pull-requests), por ju lutemi respektoni 
kufizimet e mëposhtme:

* Ju lutemi **mos** përdorni ndjekësin e problemeve për kërkesa suporti personale (përdorni 
  [Stack Overflow](http://stackoverflow.com/questions/tagged/php) ose IRC).

* Ju lutemi **mos** dilni nga tema ose të talleni me problemet. Ruajeni diskutimin brënda temës 
  dhe respektoni mendimet e te tjerëve.

<a name="pull-requests"></a>
## Pull Requests

Pull requests janë një mënyrë shumë e mirë për të shtuar përmbajtje tek PHP Mënyra e saktë, 
si dhe të përditësosh çdo problem shfletuesi ose ndryshime në stilim. Pothuajse 
çdo lloj ndryshim është i mirëpritur nëse shihet si konstruktiv. 

Ndjekja e procesit të mëposhtëm është mënyra më e mirë për të përfshirë 
punën tuaj në këtë projekt:

1. Bëni [fork](http://help.github.com/fork-a-repo/) projektin, klononi fork-un, 
   dhe konfiguroni remotes:
   
   ```bash
      # Klononi fork-un tuaj të repos në direktorinë aktuale
      git clone https://github.com/<your-username>/php-the-right-ëay.git
      # Shkoni tek direktoria e klonuar
      cd php-the-right-way
      # Jepjani repo-n origjinal një remote të quajtur "upstream"
      git remote add upstream https://github.com/anooxy/php-the-right-way.git
      ```

2. Nëse keni klonuar kohë më parë, merrni ndryshimet e fundit nga upstream:

   ```bash
   git checkout gh-pages
   git pull upstream gh-pages
   ```

3. Krijoni një branch temë të ri (prej branch-it kryesor të projektit) që 
   të permbajë ndryshimin ose rregullimin tuaj:

   ```bash
   git checkout -b <topic-branch-name>
   ```

4. Instaloni gem-in [Jekyll](https://github.com/jekyll/jekyll/) për ta parë projektin lokalisht.

5. Bëni commit ndryshimet tuaja në copëza llogjike. Ju lutem ndiqni rregullat tek 
   [git commit message guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
   përndryshe përmbajtja juaj ka shumë gjasë të mos shkrihet me projektin kryesor. Përdorni
   [interactive rebase](https://help.github.com/articles/interactive-rebase)
   të Git-it për të rregulluar commit-et tuaja para se ti bëni publike.

6. Bëni merge (ose rebase) branch-in në upstream tek branchi juaj lokalisht:

   ```bash
   git pull [--rebase] upstream gh-pages
   ```

7. Bëni push branchin tuaj tek forku juaj:

   ```bash
   git push origin <topic-branch-name>
   ```

8. [Hapni një Pull Request](https://help.github.com/articles/using-pull-requests/)
   me një titull dhe përshkrim të qartë.

## Termat e Kontribuimit dhe Përdorimi

Duke krijuar një pull request tek ky repo, ju pranoni që ti lejoni pronarëve të projektit
të licensojnë punën tuaj sipas [Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-nc-sa/3.0/).

Po e njëjta përmbajtje dhe license do përdoret per çdo publikim të PHP Mënyra e saktë, 
përfshirë këtu - dhe jo limituar tek:

* [phptherightway.com](http://phptherightway.com)
* Përkthime të phptherightway.com
* [LeanPub: PHP The Right Way](https://leanpub.com/phptherightway/)
* Përkthime të "LeanPub: PHP The Right Way"

Çdo përmbajtje do jëtë gjithmonë falas tani, dhe përgjithmonë.

## Guida Stilit për Kontribuim

1. Përdorni drejtshkrim Shqip (*vetëm për repo-n në Shqip*)
2. Përdorni katër (4) hapësira për të indent-uar tekstin; mos përdorni tab.
3. Maksimumi i një rreshti të jetë 120 karaktere.
4. Shëmbujt e kodit duhet te ndjekin standartin PSR-1 e sipër.
5. Përdorni [GitHub Flavored Markdown](http://github.github.com/github-flavored-markdown/) për cdo përmbajtje
6. Përdorni URL agnostike nga ana gjuhësore kur i referoheni faqjeve eksternal si manuali [php.net](http://php.net/urlhoëto.php)
