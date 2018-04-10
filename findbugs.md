FindBugs
http://findbugs.sourceforge.net

O FindBugs é uma das mais populares ferramentas de análise de código, sua análise é feita sobre o byte-code gerado.
Sua implementação é baseada no conceito de bug patterns, onde um determinado conjunto de códigos muitas vezes indica um erro.
Isso acontece por vários motivos, entre eles são destacados os seguintes:

    -Funcionalidades complexas da linguagem;
    - Entendimento não correto dos métodos disponíveis na API;
    - Erros do desenvolvedor: erros de digitação, uso incorreto de operadores booleanos.
    - Feita a análise, os problemas encontrados são agrupados da seguinte maneira:
    - Corretude: o código pode estar fazendo algo claramente não desejado, como referência a um objeto que pode causar Null Pointer Exception ou a chamada ao método equals() comparando classes não relacionadas;
    - Prática ruim: o código viola uma boa prática, como sobrescrever o método equals() sem sobrescrever o método hashCode() e declarar o serialVersionUUID como long, final ou static;
    - Concorrência: como uso incorreto de wait() e notify() ;
    - Performance: Uso de construtor de Integer, ao invés de Integer.valueOf(), chamada explícita ao garbage collector;
    - Código malicioso: como um campo estático declarado como um array mutável;

Veja no arquivo "eclipse.txt" sobre como configurar e usar o Findbugs no Eclipse.

Eclipse com Findbugs
1 - Instalação do plugin
_ Help->Eclipse Marketplace...
_ procure e instale o plugin do Findbugs by The University of Maryland
2 - Configuração
_ Windows->Preferences->FindBugs deixe todas no modo padrão, clicando em "Restore Defaults"
3 - Como Usar
_ Para executar o FindBugs, clique com o botão direito do mouse sobre o arquivo do projeto
FindBugs->FindBugs
_ Agora abra a perspectiva do JavaBugs, e visualize os itens na aba BugExplorer.
_ Para remover as marcações de bugs, no menu de contexto do arquivo, clique em "Clear Bugs Markers"
