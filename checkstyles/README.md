Checkstyle
http://checkstyle.sourceforge.net/

Checkstyle é uma ferramenta de análise com foco no estilo de codificação e não na lógica ou integridade do código.
Alguns pontos checados por ele: - Comprimento máximo da linha, em caracteres; - Identação por tabulações ou número de espaços; - Convenção de nomes de atributos e métodos; - Presença de javadoc em classes, atributos e métodos; - Presença obrigatória de cabeçalhos; - Limite no número de parâmetros e linhas dentro de um método; - Utilização dos pacotes e classes importadas dentro de outra classe.

Veja no arquivo "eclipse.txt" sobre como configurar e usar o Checkstyle no Eclipse.

Eclipse com checkstyle

    1 - Instalação do plugin
    	* Help->Eclipse Marketplace...
    	* procure e instale o plugin do Checkstyle by Larz Ködderitzch
    	** se tiver algum problema durante este processo, você pode tentar instalar manualmente,
    		Siga estes passos usando o arquivo do plugin: http://stackoverflow.com/questions/31553376/eclipse-how-to-install-a-plugin-manually
    		baixando o plugin aqui: https://sourceforge.net/p/eclipse-cs/
    		no eclipse-mars funciona com esta versão: 6.19
    		https://sourceforge.net/projects/eclipse-cs/files/Eclipse%20Checkstyle%20Plug-in/6.19.1/net.sf.eclipsecs-updatesite_6.19.1.201607051943.zip/download



    2 - Configuração
    	2.1 - Configuração do plugin
    		* Windows->Preference->Checkstyle
    			* Deixe marcado:
    				* Warn before losing configured file sets
    				* Include rules names in violations messages
    			* clique em New...
    				* Check Configuration
    					Type="External Configuration File",
    					Name="Custom checkstyle",
    					Localization=[caminho do arquivo custom_checks.xml]
    				* Salve a nova configuração
    		* Selecione "Custom checkstyle" e clique em "Set as Default"

    	2.4 - Quando o arquivo "custom_checks.xml" for modificado repita as operações de Configuração do plugin(2.1)

    3 - Como Usar
    	* Para fazer o check clique com o botão direito do mouse sobre o arquivo do projeto
    		Checkstyle->Check Code with Checkstyle
    	* Após o check, marcações surgirão na linhas do código caso exista alguma violação.
    		Estas violações também pode ser vistas na aba Problems.
    	* Para limpar as violações, botão direito do mouse sobre o arquivo,
    		Checkstyle->Clear Checkstyle violations
