#Laboratório de Testes com Git e Github
Este é meu laboratório para testar as funcionalidades do Git e do Github baseado nos seguintes links:

http://rogerdudler.github.io/git-guide/

http://rogerdudler.github.io/git-guide/files/git_cheat_sheet.pdf

O que eu preciso testar neste repositório é:

  . Branches + Merge
  
  . Tags
  
  . Descarte de Alterações

  . Pull Requests 

  . Gists

  . Issues


--------------------

##Branch
Uma **Branch** é uma área a parte no repositório onde você pode criar novas Features ou acertar bugs, todas as alterações feitas na Branch ficam disponíveis tanto nela mesma quanto para o **MASTER** enquanto as alterações estão no **Working Directory**, a partir do momento que as alterações são comitadas para a Branch, o MASTER não tem mais conhecimento desta alterações, neste caso para atualizar o MASTER utiliza-se o **Merge**.

###Criando uma 	Branch
Para criar uma nova **Branch** devemos utilizar o seguinte comando:
```git
git checkout -b nomeDaBranch
```
###Voltando para o MASTER
Para voltar ao MASTER digite:
```git
git checkout master
```

###Deletando a Branch recém criada:
```git
git branch -d nomeDaBranch
```

Os comando de Add e de Commit na Branch são os mesmos do MASTER.

--------------------

###Diff
O comando **diff** lista as diferenças entre uma branch e outra ou mesmo de uma só branch, exemplo:
#####Diferenças de arquivos na Branch Atual:
```git
git diff
```

#####Diferenças de Arquivos entre a Branch MASTER e a novaBranch:
```git
git diff master novaBranch
```

--------------------

###Merge
O **Merge** junta as alterações feitas na Branch com o MASTER, caso hava alguma inconsistência você deverá alterar manualmente os arquivos listados. O **Merge** deverá ser feito na Branch de destino, exemplo se quiser fazer um Merge da novaBranch para o MASTER, digite o seguinte:
```git
git checkout master //muda para o master
git merge novaBranch
```


