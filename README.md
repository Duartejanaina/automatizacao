Gerador de PDF e Envio de Email para Quadro de Referência Provisória (QRP)

Descrição

Este script automatiza a geração de um PDF contendo informações extraídas de uma planilha do Google Sheets e realiza o envio do arquivo por e-mail. Ele utiliza bibliotecas como pandas, fpdf, gspread e smtplib para manipulação de dados, criação de documentos e envio de e-mails.

Funcionalidades

Autentica e acessa uma planilha no Google Sheets

Processa os dados extraídos e filtra o código QRP mais recente

Gera um PDF com as informações formatadas

Implementa tentativas automáticas de reconexão em caso de falha na API do Google Sheets

Envia o PDF gerado para destinatários via e-mail

Dependências

Antes de executar o script, instale as seguintes bibliotecas:

pip install pandas fpdf gspread schedule smtplib

Configuração

Credenciais do Google Sheets

Configure um arquivo JSON com credenciais de serviço do Google.

Substitua "caminho.json" pelo caminho correto do arquivo JSON.

ID da Planilha

Substitua "planilha ID" pelo ID da sua planilha no Google Sheets.

Substitua "Nome da aba" pelo nome da aba correta na planilha.

Envio de Email

Configure um e-mail remetente e sua senha.

Altere os destinatários na variável destinatarios.

Uso

Execute o script com:

python script.py

Estrutura do Código

Classe MyPDF: Define o cabeçalho e rodapé do PDF.

Autenticação no Google Sheets: Conecta-se à planilha e extrai os dados.

Geração do PDF: Processa os dados do QRP e cria um arquivo PDF.

Função tarefa: Implementa tentativas de reconexão ao Google Sheets em caso de falha.

Função enviar_email: Envia o PDF gerado para os destinatários.

Observações

O script é projetado para rodar periodicamente, gerando e enviando PDFs automaticamente.

Certifique-se de que a autenticação do e-mail esteja configurada corretamente para evitar bloqueios de envio.

Autor

Desenvolvido para automação de relatórios de QRP e envio de comunicações automatizadas via e-mail.
