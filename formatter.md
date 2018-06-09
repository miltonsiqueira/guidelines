Procedimento para aplicar uma formatação padrão para o código fonte em Java.
Para usar no Eclipse, acesse arquivo "eclipse.txt"

Formatter no Eclipse baseado no checkstyle
1 - Configurao
_ Windows->Preference->Java->Code Style->Formatter
_ Clique em Import, escolha o arquivo "eclipse*formatter.xml"
* Deixe o novo formatter "eclipse-cs custom" como "Active profile"
2 - Utilizao
\_ Dentro da janela do arquivo java faa: Ctrl + Shift + F

    3 - (Opcional) Formatar automaticamente ao salvar arquivo
    	* Windows->Preference->Java->Editor->Save Actions
    	* Deixe marcado
    		Perform the selected actions on save
    		Format source code
    		Format all lines
    		Organize imports
    		Additional actions
    			Configure...
    				Aba Code Organizing -> todos desmarcados
    				Code style -> todos desmarcados
    				Member accesses -> todos desmarcados
    				Missing code ->
    					todos marcados (Add missing Annotations, @Override, Implement...1.6 or higher), @Deprecated
    				Unnecessary Code ->
    					marque: Remove unused imports, Remove unused local variables, Remove unnecessary casts

    4 - (Opcional) Criando novo formatter baseado no checkstyle
    	* Boto direito no projeto->Checkstyle->Create Formatter-Profile
    	* Windows->Preference->Java->Code Style->Formatter
    	* Selecione "eclipse-cs idw" e clique em "Edit..."
    	* Renomeie o formatter gerado de "eclipse-cs idw" para "eclipse-cs custom"
    	* Indentation->General Settings->Tab policy: "Tab only"
    	* Line wrapping->General Settings->marque "Never join already wrapped lines"
    	* Deixe o formatter "eclise-cs custom" selecionado e clique ok
    	* Quando o arquivo "custom_checks.xml" for modificado repita as operaes de Configurao do plugin(2.1) e de criao do formatter(2.2)
