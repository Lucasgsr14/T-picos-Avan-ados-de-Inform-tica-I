# Tópicos-Avançados-de-Informática-I

## Instruções para criar a sua base de dados com várias imagens

Para criar sua base de dados é só colocar suas imagens na pasta e renomear-lá para fica no formato "imgN.jpg" onde N deve ser substituido pelo número da imagem que você deseja, desde que a contagem parta da o 1 ao número desejado sem pular nenhum número.\
Existem duas mudanças necessárias no código:
* A primeira é informar qual o número de imagens que serão processadas na variável "nImgs".
```javascript
    var nImgs = ;
```
* A segunda é o preenchimento do vetor de estados de acordo com as posições das fotos. Como exemplo:
```javascript
    var arrEstados = ["levantado", "sentado", "levantado", "sentado", "sentado"];
```
O passo final é copiar o texto foi gerado na página acessada quando se clica no icone "index.html", jogar o texto copiado no bloco de notas e salvar seu arquivo com a extensão "*.csv".

## Dicas para gerar imagens a partir de um vídeo (**MÉTODO APENAS PARA USUÁRIOS DE UBUNTU**)

Para conseguir extrair imagens de um video, o que é bem mais simples que selecionar imagens aleatórias de pessoas em pé e sentadas, podemos usar o comando:\
`$ ffmpeg -i video.mp4 -r N img%d.jpg`\
onde `video.mp4` é o nome do seu arquivo de vídeo e `N` é o número inteiro de frames por segundo de vídeo.\
> Lembrar de que o comando deve ser executado da pasta onde o vídeo está e as imagens serão geradas nessa mesma pasta
