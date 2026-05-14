# Agência Classe A — Site Institucional

Site institucional profissional da **Agência Classe A**, empresa de distribuição de panfletos e flyers em São Paulo desde 2008.

## Visão Geral

- **Tecnologia:** HTML5 + CSS3 + JavaScript puro (sem frameworks)
- **Arquitetura:** Single-file (`index.html`) — tudo em um arquivo
- **Deploy:** GitHub Pages / Netlify Drop
- **Domínio:** agenciaclassea.com.br (Registro.br)

## Estrutura de Arquivos

```
Site/
├── index.html              ← Site completo (HTML + CSS + JS)
├── .gitignore
├── README.md
└── img/
    ├── logo-classe-a.png
    ├── secao-nossos-servicos/
    │   ├── porta-a-porta.png
    │   ├── farol-ponto-fixo.png
    │   ├── panfletagem-em-comercios.png
    │   ├── acoes-especiais.png
    │   ├── mala-direta-sampling.png
    │   └── cobertura-sp-interior.png
    ├── secao-clientes/
    │   ├── roldao-atacadista.png
    │   ├── assai-atacadista.png
    │   ├── oxxo.png
    │   └── ... (14 logos)
    └── secao-portfolio/
        ├── roldao/equipe-roldao.jpg
        ├── estadao/equipe-estadao.png
        └── assai/
            ├── equipe-assai.jpeg
            └── assai-dia-das-maes.jpeg
```

## Seções do Site

1. **Navbar** — Fixa, responsiva, com menu hambúrguer no mobile
2. **Hero** — Efeito de digitação animado, contadores, CTA duplo
3. **Sobre** — Institucional + 4 diferenciais
4. **Serviços** — 6 cards com fotos reais e efeito shine
5. **Processo** — 4 etapas de trabalho
6. **Tecnologia** — Geofusion + We Trade
7. **Diferenciais** — Estatísticas animadas + lista de vantagens
8. **Equipes** — Dados da equipe + contatos Lindsay e Guilherme
9. **Portfólio** — Fotos reais com lightbox interativo
10. **Clientes** — Marquee infinito com 14 logos
11. **Depoimentos** — 3 cards de clientes
12. **FAQ** — 5 perguntas com acordeão
13. **Contato** — Formulário → WhatsApp + botões diretos
14. **Footer** — Links + Google Maps embutido

## Funcionalidades Técnicas

- Scroll progress bar
- Reveal animations (IntersectionObserver)
- Contadores animados (requestAnimationFrame)
- Efeito de digitação (typewriter)
- Card shine effect (mousemove)
- Marquee infinito de logos
- Lightbox no portfólio (navegação por teclado)
- Máscara de telefone no formulário
- Formulário com validação e envio via WhatsApp
- Menu mobile com aria-expanded
- Google Maps embutido

## Deploy no GitHub Pages

1. Crie um repositório no GitHub (ex: `agencia-classe-a-site`)
2. Faça upload dos arquivos:
   ```bash
   git init
   git add .
   git commit -m "Lançamento do site Agência Classe A"
   git remote add origin https://github.com/SEU_USUARIO/agencia-classe-a-site.git
   git push -u origin main
   ```
3. Vá em **Settings > Pages > Source: main / root**
4. Seu site estará em: `https://seu-usuario.github.io/agencia-classe-a-site/`

## Deploy no Netlify (recomendado)

1. Acesse [netlify.com](https://netlify.com) e faça login
2. Clique em **"Add new site" > "Deploy manually"**
3. Arraste a pasta `Site/` para a área indicada
4. Pronto — URL gerada em segundos (ex: `classe-a.netlify.app`)

## Configuração de Domínio (Registro.br)

1. Compre o domínio em [registro.br](https://registro.br)
2. No painel do Netlify/GitHub Pages, copie o IP ou CNAME fornecido
3. No Registro.br, acesse **DNS > Editar zona**:
   - Tipo **A** → IP do Netlify (`75.2.60.5`)
   - Tipo **CNAME** → `www` → `seu-site.netlify.app`
4. Aguarde propagação DNS (até 48h, normalmente menos de 1h)
5. HTTPS é ativado automaticamente pelo Netlify (Let's Encrypt)

## Contatos

- **Comercial:** Lindsay — (11) 97731-3911
- **Atendimento:** Guilherme — (11) 98515-6903
- **Endereço:** Rua Dias Coelho, 253 · São Paulo, SP

---

*Desenvolvido em 2025. Todos os direitos reservados à Agência Classe A.*
