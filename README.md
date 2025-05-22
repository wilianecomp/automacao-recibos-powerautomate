# 📄 Projeto 1 – Automação de Envio de Recibos com Excel e Power Automate

## 🧩 Descrição do problema

Profissionais autônomos, como psicólogos, consultores e personal trainers, precisam frequentemente enviar recibos por e-mail após cada atendimento. O processo manual envolve abrir planilhas, copiar dados, escrever e-mails personalizados e acompanhar quem já recebeu. É demorado, repetitivo e propenso a erros.

---

## ✅ Solução criada

Desenvolvi uma automação utilizando **Excel Online + Power Automate**, que envia e-mails com recibos automaticamente assim que os dados são preenchidos na planilha.

---

## 🛠️ Ferramentas utilizadas

- Microsoft Excel (armazenado no OneDrive)
- Power Automate (Microsoft)
- Outlook (envio de e-mails)
- Conta Microsoft gratuita

---

## 🔁 Funcionamento do fluxo

1. O profissional preenche uma **linha da planilha Excel** com:
   - Nome do cliente
   - E-mail do cliente
   - Data do atendimento
   - Valor pago
   - Forma de pagamento
   - Status (campo que começa vazio)

2. O Power Automate detecta uma nova linha com “Status = vazio”

3. O robô:
   - Gera automaticamente um texto de recibo personalizado
   - Envia o e-mail via Outlook com os dados preenchidos
   - Atualiza o campo “Status” na planilha para “Enviado”

---

## ✉️ Exemplo do e-mail enviado

Assunto: Recibo de Atendimento - João Silva

Olá João,

Segue o recibo referente ao atendimento do dia 12/05/2025, no valor de R$ 150,00.

Forma de pagamento: Pix.

Qualquer dúvida, fico à disposição.

Atenciosamente,
Wilian Cardoso
Automação Digital


---

## 📁 Arquivos incluídos

- `modelo-planilha.xlsx` – Planilha com colunas e exemplo preenchido
- `print-fluxo.png` – Captura de tela do fluxo no Power Automate
- `fluxo-comentado.pdf` – Explicação em passos do funcionamento do fluxo
- (Opcional) `video-demo.mp4` – Gravação do fluxo rodando (se quiser)

---

## 🚀 Como testar ou adaptar

1. Faça login em uma conta Microsoft
2. Suba a planilha `modelo-planilha.xlsx` no seu OneDrive
3. Crie um fluxo no Power Automate usando o gatilho:
   - **“Quando uma linha é adicionada/modificada em uma tabela (Excel Online)”**
4. Configure as ações conforme descritas no `fluxo-comentado.pdf`
5. Teste inserindo uma nova linha com os dados fictícios
6. Verifique se o e-mail chegou e se o campo "Status" mudou para “Enviado”

---

## 🧠 O que essa automação resolve

- Reduz tempo gasto com tarefas manuais
- Evita erros de digitação ou esquecimentos
- Padroniza a comunicação com os clientes
- Permite escalar o atendimento sem perder qualidade

---

## 📌 Próximos passos

Em breve, este mesmo projeto será adaptado usando **Google Sheets + AppSheet**, permitindo uso em celulares sem depender de Power Automate.

---

Desenvolvido por [Wilian Cardoso](mailto:wilianecomp@gmail.com)  
Especialista em automação de tarefas digitais
