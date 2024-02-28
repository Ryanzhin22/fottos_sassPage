# fottos_sassPage
 Uma página criada para testar a extesão da linguagem CSS, A Sass e grande parte do que ela tem a oferecer.

SASS

-> O navegador não lê um arquivo .sass portanto é necessário compilar esse mesmo arquivo e transforma-lo em CSS
-> Essa compilação vai ser feita por meio do comando sass --watch sass/styles.sass:css/styles.css

VARIÁVEIS
-> O SASS pode armazenar variáveis em um arquivo chamado "_variables.sass"
-> Para importar é só fazer a importação do arquivo usando @use 'variables'
-> Para usar uma variável é só fazer "color: variables.$primaryColor"

MIXINS
-> Os mixins servem para criar "funções com comandos css"
-> @mixin container -> max-width: variables.$containerWidth, padding: 1rem 0, margin: 0 auto
-> Ao utilizar o comando acima no arquivo principal da seguinte forma: @include mixins.container, todos os arquivos com esse código terão os atributos acima
-> Também é possível criar um mixin para uma resolução específica para responsividade

-------------------------------------------------

-> Ao criar duas classes, uma principal chamada .header e outra como .headerBrand dentro da principal, chamá-las no sass é muito mais fácil
-> Chame primeiro a principal e estilize-a, em sequencia para chamar a próxima basta usar &Brand e estilizar a classe .headerBrand
-> O & completa no arquivo o "header"
