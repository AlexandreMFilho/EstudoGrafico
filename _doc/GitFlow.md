### Iniciando um rep GitFlow

https://danielkummer.github.io/git-flow-cheatsheet/

https://www.gitkraken.com/learn/git/git-flow


Para iniciar um repositório GitFlow, pode-se pegar um repositório git já criado ou de uma pasta não iniciada no git e digitar o seguinte comando bash:

```
git flow init
``` 
Este comando irá iniciar o repositório no GitFlow onde será possível realizar algumas configurações iniciais dos nomes das branchs que serão usadas como pode ser visto abaixo.

![Alt text](image.png)

Ao ser inicializado o git flow, criará a branch master e a develop e ja te colocará na branch develop.

Aqui será onde o trabalho desenvolvido será armazenado.

Para iniciar um feature basta usar o comando:

```
git flow feature start [NomeDaFeature]
```
![Alt text](image-1.png)

Uma branch ``Feature/[NomeDaFeature]`` será criada e você será jogado nela.
Após realizar o trabalho, basta dar :

```
git add .
git commit -m "Seu commit"
```

Caso ainda haja algum trabalho a ser feito, a feature pode ser publicada com o comando ;

```
git flow feature publish [NomeDaFeature]
```

Ao concluir a feature basta finaliza-la com o comando:

```
git flow feature finish [NomeDaFeature]
```

Será solicitado a adição de uma explicação do trabalho realizado, como um commit explicando o motivo do merge.
Finalizando você voltará para a develop atualizada com a feature que foi finalizada.

![Alt text](image-2.png)
