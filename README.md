#Nyttiga gitkommandon

## Ta ut en ny branch lokalt
git checkout -b <namnpåbranch>

## Checka ut befintlig branch
git checkout <branchnamn>

## Lägg till alla filer för commit
git add *

## Lägg till specifik fil för commit
git add index.html

## Skapa commit
git commit -m "LABB-0001 Någon fin beskrivning"

## Pusha commit och sätt upstream (behöver göras första gången om du skapar branchen lokalt)
git push -u origin HEAD

## Pusha commit i branch som redan har upstream satt
git push

## Rebase - Ta in ändringar från master till din featurebranch
git checkout main
git pull
git checkout <featurebranch som du vill rebasa>
git rebase
Om inga konflikter uppstod: git push --force
