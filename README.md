# Visualizador-de-Dados-IA-com-Gemini-2.5-Flash-V2
Página que recebe dados externos em JSON e gera descrições e gráficos com modelo LLM

<img src="Captura de tela 2025-11-10 090519.png">

<h1>Funcionamento</h1>

<h2>Google Sheets</h2>
o código do google sheets possui três funções:
<b>getSheetData</b> responsável por pegar os dados da planilha e converter em JSON
<b>doGet</b> retorna os dados JSON para o site ou qualquer outro sistema que acessar a aplicação
<b>doPost</b> recebe dados de fora, esp32 por exemplo, e insere na planilha

<h2>ESP32</h2>
lê os dados de um sensor e manda para a planilha

<h2>Site</h2>
pega os dados da planilha e envia um prompt para o modelo Gemini 2.5 Flash pra gerar gráficos e descriçoes personalizadas
