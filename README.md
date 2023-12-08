# FIELD-MODULE-ON-INPUT
No contexto do ABAP (Advanced Business Application Programming), "FIELD", "MODULE", "ON INPUT", "PAI" e "PBO" são termos relacionados à programação de telas (Dynpros). Vamos abordar cada um deles:

1. **FIELD**:
   - No ABAP, o comando `FIELD` é usado para definir um campo de tela específico.
   - Ele é frequentemente usado em módulos de tela para manipular o conteúdo de campos.

   Exemplo:
   ```abap
   FIELD my_field MODULE module_name.
   ```

2. **MODULE**:
   - Um módulo no ABAP é uma unidade lógica de código que executa uma função específica.
   - Em programação de tela (Dynpros), os módulos são frequentemente usados para controlar eventos específicos, como a entrada de dados (ON INPUT), carregamento de dados na tela (PBO - Process Before Output) e processamento de eventos de usuário (PAI - Process After Input).

   Exemplo de uso de MODULE:
   ```abap
   MODULE module_name OUTPUT.
     " Código para preparar a tela (PBO - Process Before Output)
   ENDMODULE.

   MODULE module_name INPUT.
     " Código para processar a entrada do usuário (PAI - Process After Input)
   ENDMODULE.
   ```

3. **ON INPUT**:
   - `ON INPUT` é uma cláusula usada em módulos de tela para lidar com eventos associados à entrada do usuário.
   - Quando um usuário insere dados em campos de tela, o código dentro de um módulo `ON INPUT` é executado para processar essa entrada.

   Exemplo:
   ```abap
   MODULE module_name INPUT.
     " Código para processar a entrada do usuário (ON INPUT)
   ENDMODULE.
   ```

4. **PAI (Process After Input)**:
   - É um tipo de módulo de tela que é executado após o usuário interagir com a tela (por exemplo, após pressionar Enter).
   - O código PAI é usado para processar a entrada do usuário e realizar ações com base nos dados inseridos.

   Exemplo:
   ```abap
   MODULE module_name INPUT.
     " Código para processar a entrada do usuário (PAI - Process After Input)
   ENDMODULE.
   ```

5. **PBO (Process Before Output)**:
   - É um tipo de módulo de tela que é executado antes da exibição da tela.
   - O código PBO é usado para preparar a tela, preenchendo campos com dados iniciais ou realizando outras tarefas antes da exibição.

   Exemplo:
   ```abap
   MODULE module_name OUTPUT.
     " Código para preparar a tela (PBO - Process Before Output)
   ENDMODULE.
   ```

Estas são algumas noções básicas sobre os termos mencionados no contexto do ABAP e da programação de telas. O ABAP é uma linguagem de programação voltada para o desenvolvimento de sistemas SAP, e esses conceitos são específicos para a interação do usuário com as telas do sistema.
