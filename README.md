# Projeto Loteca
Este é um projeto de simulador de loteria, 
onde o usuário digita 6 números e realiza um sorteio de outros 6  números, 
logo é verificado quantos números ele acertou

## Tecnologias utilizadas
- **HTML**: estrutura do site
- __CSS__: Estilização do site
- *_JS_*: funções do site

### Melhorias possíveis
1. [X] Subir para GitHubPages
2. [ ] Alterar os alerts
3. [ ] Utilizar o Bootstrap
4. [ ] Deixar responsivo

### Disponibilizado em
[GitHubPage](https://renanberserk.github.io/loteca/)

### Prints da tela

  | ID | Primeira tela | Segunda Tela     |
  |----|---------------|------------------|
  |  1 | loteca Limpa  | loteca Preenchida|
  |  2 |![image](https://user-images.githubusercontent.com/100212335/162979264-69779393-6f38-458a-9398-093d2917201c.png) | ![Tela sorteada](https://user-images.githubusercontent.com/100212335/162984538-9e4945d2-40e1-4fa4-b679-ef02457a94c2.png) |




#### Função Pricipal
```Js:
function sorteio() {
  if(numEsco.length == 6){
  var cont = 0;
  numSort = [];

  while (cont < 6) {
    let num = Math.random() * 60;
    num = Math.ceil(num);
    if (!numSort.includes(num)) {
      numSort[cont] = num;
      console.log(numSort);
      cont++;
    }
  }
  
  document.getElementById("sorteados").innerHTML = numSort;
  contAcertos();
} else {
  alert("É necessario digitar seis numeros antes do sorteio")

}
}
```
  
### comando git
Para iniciar o projeto
```bash
git init
```
