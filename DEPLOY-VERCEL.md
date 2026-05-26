# 🚀 Como Subir a Apresentação na Vercel

> **Tempo estimado: 3 a 5 minutos**  
> Repositório: [joaozinho0035/portugues-apresentacao-generos-textuais](https://github.com/joaozinho0035/portugues-apresentacao-generos-textuais)

---

## Pré-requisitos

- ✅ Conta no GitHub (já feita: `joaozinho0035`)
- ✅ Repositório no GitHub (já criado e com código)
- Uma conta na Vercel (gratuita — pode entrar com o próprio GitHub)

---

## Passo a Passo

### 1. Acessar a Vercel

Abra o navegador e acesse:

```
https://vercel.com
```

---

### 2. Fazer Login

Clique em **"Log In"** (canto superior direito).

Na tela de login, escolha:

> **"Continue with GitHub"**

Autorize a Vercel a acessar seu GitHub. Isso vincula as duas contas automaticamente.

---

### 3. Importar o Repositório

Após o login, você verá o **dashboard** da Vercel.

1. Clique no botão **"Add New…"** → selecione **"Project"**
2. Na seção **"Import Git Repository"**, procure pelo repositório:

   ```
   portugues-apresentacao-generos-textuais
   ```

3. Clique em **"Import"** ao lado do repositório.

---

### 4. Configurar o Projeto

Na tela de configuração do projeto, preencha assim:

| Campo | Valor |
|-------|-------|
| **Framework Preset** | `Other` (não é Next.js, nem React) |
| **Root Directory** | `.` (ponto — deixar padrão) |
| **Build Command** | *(deixar vazio)* |
| **Output Directory** | `.` (ponto — raiz do projeto) |

> ⚠️ **Importante:** Certifique-se de que o **Output Directory** está como `.` (ponto). Isso diz à Vercel para servir os arquivos da raiz do repositório.

O arquivo `vercel.json` já está configurado no repositório para redirecionar a URL raiz (`/`) para a `presentation.html`.

---

### 5. Fazer o Deploy

Clique no botão **"Deploy"** (azul, no final da página).

A Vercel vai:
1. Baixar o repositório do GitHub
2. Detectar que é um site estático
3. Subir todos os arquivos
4. Gerar uma URL pública

⏳ **Aguarde cerca de 30 a 60 segundos.**

---

### 6. Acessar a Apresentação

Quando o deploy terminar, a Vercel vai exibir:

```
🎉 Congratulations! Your project has been deployed.
```

E uma URL do tipo:

```
https://portugues-apresentacao-generos-textuais.vercel.app
```

Clique nessa URL para abrir a apresentação no navegador. ✅

---

## Dicas para a Apresentação

### Modo Tela Cheia
- Pressione **`F`** para entrar em tela cheia dentro da apresentação
- Ou pressione **`F11`** no navegador para fullscreen total

### Navegar pelos Slides
| Ação | Tecla |
|------|-------|
| Próximo slide | `→` ou `Espaço` |
| Slide anterior | `←` |
| Sair do fullscreen | `Esc` |

### Compartilhar o Link
Você pode enviar a URL da Vercel para a professora ou colegas assistirem de qualquer dispositivo — celular, tablet ou computador.

---

## Estrutura dos 6 Slides

| # | Título | Conteúdo |
|---|--------|----------|
| 01 | **Abertura** | Título, subtítulo, tema da apresentação |
| 02 | **O que são Gêneros Textuais** | Conceito + lista de gêneros |
| 03 | **Mercado de Trabalho** | 5 profissões e seus gêneros |
| 04 | **Impacto Profissional** | A comunicação abre portas |
| 05 | **Exemplos na Prática** ⭐ | Email, Petição, Artigo, Notícia, Relatório |
| 06 | **Conclusão** | "Comunicação é poder" |

---

## Solução de Problemas

### A página abre em branco ou com erro 404
Verifique se o **Output Directory** foi configurado como `.` (ponto) nas configurações do projeto na Vercel. Você pode alterar em:

`Dashboard → Projeto → Settings → Build & Development Settings`

### As fontes não carregam
A apresentação usa fontes do Google Fonts. Verifique se o dispositivo tem acesso à internet. As fontes são carregadas dos arquivos locais (`finex-finance-saas.aura.build/assets/`) para garantir funcionamento offline.

### Quer atualizar a apresentação depois
Se fizer alterações no arquivo `presentation.html`, basta rodar no terminal:

```bash
git add presentation.html
git commit -m "atualiza apresentação"
git push
```

A Vercel detecta automaticamente o push e faz o **redeploy** em menos de 1 minuto.

---

## Links Úteis

- 🔗 **Repositório GitHub:** https://github.com/joaozinho0035/portugues-apresentacao-generos-textuais
- 🌐 **Vercel:** https://vercel.com
- 📚 **Documentação Vercel (static sites):** https://vercel.com/docs/frameworks/more-frameworks

---

*Boa apresentação amanhã! 🎓*
