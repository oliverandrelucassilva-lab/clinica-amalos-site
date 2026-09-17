# Clínica Amalos — Landing Page

Site institucional de uma página para a Clínica Amalos (Saúde Integrativa e Odontológica), em Euclides da Cunha, BA.

## Estrutura

- `index.html` — todas as seções da página (Hero, Sobre, Especialidades, Diferencial, Agenda, Depoimentos, Localização, CTA final)
- `css/style.css` — identidade visual (rosa pastel + coral/pêssego), responsiva e mobile-first
- `js/script.js` — menu mobile e pequenas interações
- `assets/img/` — pasta para imagens do site

## Foto da Dra. Edivânia (hero)

O hero foi montado para exibir a foto da Dra. Edivânia. Adicione o arquivo da foto em:

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
