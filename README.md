# Orçamento de Impressão 3D - Uso Pessoal

Ferramenta em HTML criada para meu uso pessoal, que calcula o custo de impressões 3D a partir de arquivos **.gcode** gerados no OrcaSlicer.  
O sistema lê automaticamente informações importantes e gera uma mensagem pronta para envio no WhatsApp.

## 🔹 Informações extraídas automaticamente do G-code
- Nome da peça
- Tempo estimado de impressão
- Peso do filamento
- Miniatura (se disponível)

## 🔹 Funcionalidades
- Preenchimento automático ao importar o G-code
- Cálculo de custo considerando filamento, energia, margem e modelagem
- Geração de mensagem pronta para WhatsApp com todas as informações
- Suporte a miniaturas 300x300 geradas pelo OrcaSlicer

---

## ⚙️ Configuração necessária no OrcaSlicer

Para que a extração funcione corretamente:

1. **Miniatura no G-code**
   - Ative nas configurações para salvar **PNG 300x300**.

2. **Formato do nome do arquivo**
   - Em **G-code file name format**, use:
     ```
     {input_filename_base}_{print_time}_{printer_preset}_{filament_preset[0]}_{filament_type[0]}.gcode
     ```

---

## 🚀 Como usar
1. Abra o arquivo `index.html` no navegador **ou** acesse a versão online no GitHub Pages:
   ```
   https://gfbarreto.github.io/orcamento-3d/
   ```
2. Clique em **Importar G-code** e selecione o arquivo.
3. Confira as informações extraídas automaticamente.
4. Clique em **Calcular** para gerar a mensagem do WhatsApp.
5. Envie para o cliente.

---

## 📄 Licença
Este projeto é para **uso pessoal**. Pode ser adaptado livremente, mas sem garantia de funcionamento para todos os cenários.
