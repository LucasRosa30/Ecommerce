**Resumo do Projeto: Loja de E-commerce (LRCOMMERCE) de Eletrônicos em Next.js e Node.js**

O projeto “LRCOMMERCE” é uma loja de e-commerce desenvolvida com Next.js, Node.js e MySQL. A aplicação, que inclui um painel administrativo completo, é totalmente personalizada e responsiva. Foi criada como parte de um TCC de um curso técnico.

**1. Recursos Chave do LRCOMMERCE**

O LRCOMMERCE é uma loja de e-commerce full-stack com painel administrativo, totalmente open-source e responsiva.

**2. Instruções para Execução**

1. **Instalar Node.js e npm:** [Tutorial de Instalação](https://www.youtube.com/watch?v=4FAtFwKVhn0) e [Download](https://nodejs.org/en).
2. **Instalar MySQL:** [Tutorial de Instalação](https://www.youtube.com/watch?v=BxdSUGBs0gM&t=212s) e [Download](https://dev.mysql.com/downloads/installer/).
3. **Baixar o projeto e extrair.**
4. **Criar arquivo `.env` na pasta raiz.**
5. **Você precisa colocar o seguinte código no arquivo .env e em vez de nome de usuário e senha coloque seu nome de usuário e senha do MySQL:**
   
     `DATABASE_URL="mysql://username:password@localhost:3306/singitronic_nextjs"`
  
     `NEXTAUTH_SECRET=12D16C923BA17672F89B18C1DB22A`
  
     `NEXTAUTH_URL=http://localhost:3000`

7. **Depois de fazer isso, você precisa criar outro arquivo `.env` na pasta `server` e colocar o mesmo DATABASE_URL usado no arquivo `.env` anterior:**

     `DATABASE_URL="mysql://username:password@localhost:3306/singitronic_nextjs"`
   
9. **Instalar dependências:** No terminal, executar `npm install` na raiz e `cd server` seguido de `npm install` na pasta do servidor.
10. **Executar migrações Prisma:** `npx prisma migrate dev` na pasta `server`.
11. **Inserir dados de exemplo:** `node insertDemoData.js` na pasta `server/utills`.
12. **Iniciar o backend:** `node app.js` na pasta `server`.
13. **Iniciar o frontend:** `npm run dev` na pasta raiz.
14. **Acessar a aplicação:** Visite [http://localhost:3000](http://localhost:3000) para ver a loja em funcionamento.
