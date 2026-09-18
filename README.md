# Clínica Amalos — Landing Page

Site institucional de uma página para a Clínica Amalos (Saúde Integrativa e Odontológica), em Euclides da Cunha, BA.

## Estrutura

- `index.html` — todas as seções da página (Hero, Sobre, Especialidades, Diferencial, Agenda, Depoimentos, Localização, CTA final) + meta tags de SEO e dados estruturados (Schema.org)
- `css/style.css` — identidade visual (rosa pastel + coral/pêssego), responsiva e mobile-first
- `js/script.js` — menu mobile e pequenas interações
- `assets/img/` — pasta para imagens do site
- `robots.txt` / `sitemap.xml` — arquivos para indexação no Google

## Foto da Dra. Edivânia (hero)

O hero foi montado para exibir a foto da Dra. Edivânia. O arquivo da foto fica em:

```
assets/img/dra-edivania-hero.jpg
```

Enquanto o arquivo não existir, um placeholder ilustrado (fundo rosa/pêssego com coração) aparece automaticamente no lugar da foto, então o site nunca fica quebrado — basta trocar a imagem quando disponível.

## Como visualizar

Basta abrir `index.html` em um navegador, ou servir a pasta com qualquer servidor estático:

```bash
python3 -m http.server 8000
```

## Personalização rápida

- **Cores**: variáveis no topo de `css/style.css` (`--pink-*`, `--peach-*`, `--gold-*`).
- **WhatsApp**: número usado nos links `wa.me` é `5575999495083` — atualize em `index.html` se necessário.
- **Mapa**: embed do Google Maps usa o endereço da clínica via busca (sem necessidade de chave de API).

## SEO — o que já está implementado

- `<title>` e `<meta description>` otimizados com palavras-chave locais (dentista infantil, odontopediatria, clínica odontológica em Euclides da Cunha).
- Open Graph e Twitter Card, para que o link fique bonito quando compartilhado no WhatsApp/Instagram/Facebook.
- Dados estruturados (Schema.org, tipo `Dentist`) com endereço, telefone, horário, especialidades e as avaliações reais — ajuda o Google a exibir estrelas e informações ricas no resultado de busca.
- `robots.txt` e `sitemap.xml` para facilitar a indexação.
- Foto do hero otimizada (de 1,6MB para ~180KB) para carregar mais rápido — velocidade de carregamento é um fator direto de ranqueamento.

### O que falta fazer *fora* do código para realmente brigar pelo 1º lugar

Nenhum site sozinho garante 1º lugar — o Google também avalia sinais fora do código:

1. **Google Perfil da Empresa (Google Business Profile)** — é o fator mais importante para aparecer no mapa/"Google Local Pack" quando alguém busca "dentista em Euclides da Cunha". Precisa reivindicar/otimizar o perfil, manter categoria, fotos, horário e posts atualizados.
2. **Avaliações no Google** — continuar pedindo aos pacientes para avaliar (já temos 4 ótimas, mas quanto mais recentes e frequentes, melhor).
3. **Citações locais (NAP consistente)** — o nome, endereço e telefone da clínica devem estar idênticos em outros diretórios (Google, Facebook, listas locais da Bahia, etc.).
4. **Cadastrar o site no Google Search Console** — enviar o `sitemap.xml` manualmente lá para acelerar a indexação e monitorar erros.
5. **Domínio próprio** (ex: `clinicaamalos.com.br`) passa mais confiança que um subdomínio `.vercel.app` — vale considerar no futuro.
6. **Backlinks locais** — parcerias, matérias em sites de notícias/blogs de Euclides da Cunha linkando para o site.
