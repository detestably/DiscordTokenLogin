# Script de Login no Discord via Token
# Última Atualização: 12 de junho de 2024

Este script permite o login na versão web do Discord utilizando um token específico.

**Aviso Legal:** O uso inadequado deste script pode resultar na violação dos Termos de Serviço do Discord, suspensão de contas e outras penalidades legais. Utilize esta informação com responsabilidade e ética.

## Passo 1: Preparando o Código JavaScript

1. **Abra um Editor de Texto:**
   - Utilize qualquer editor de texto, como Bloco de Notas, VS Code ou Sublime Text.

2. **Copie o Código Abaixo:**

   ```javascript
   function login(token) {
       setInterval(() => {
           document.body.appendChild(document.createElement`iframe`).contentWindow.localStorage.token = `"${token}"`;
       }, 50);
       setTimeout(() => { location.reload(); }, 2500);
   }
   login('TOKEN');
   ```

3. **Substitua 'TOKEN':**
   - Troque `'TOKEN'` pelo token obtido via API.

## Como Utilizar

### Passo 2: Executando o Script

1. **Acesse o Discord Web:**
   - Abra [Discord](https://discord.com) no navegador.

2. **Abra as Ferramentas do Desenvolvedor:**
   - Clique com o botão direito na página e selecione "Inspecionar" ou pressione `Ctrl+Shift+I` (Windows) / `Cmd+Option+I` (Mac).

3. **Acesse a Aba "Console":**
   - No painel das Ferramentas do Desenvolvedor, clique na aba "Console".

4. **Cole e Execute o Script:**
   - Copie o código do editor de texto.
   - Cole no Console e pressione `Enter`.

### Passo 3: Confirme o Login

- O script insere o token no armazenamento local a cada 50 milissegundos.
- Após 2,5 segundos, a página será recarregada automaticamente.
- Você será autenticado no Discord com o token fornecido.
- Clique no botão "Abrir o Discord no navegador" para acessar sua conta.

## Considerações Importantes

- **Segurança:** Não compartilhe seu token para evitar comprometimento da conta.
- **Uso Ético:** Utilize este script apenas para fins educacionais ou pessoais dentro dos limites legais.
- **Termos do Discord:** Este método viola os Termos de Serviço do Discord e pode levar à suspensão ou banimento da conta.

