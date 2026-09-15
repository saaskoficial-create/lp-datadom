# Landing page DataDom

LP da DataDom no mesmo framework Astro modular usado pelo site SMSMais, adaptada ao briefing ClickUp `86e2rhw2q` e às capturas de interface do cliente.

A versão humanizada usa duas imagens ilustrativas de profissionais de contabilidade geradas para a página. O hero e a seção de rotina foram reorganizados a partir do ritmo aberto e do foco em pessoas da LP SMSMais; as telas reais do produto continuam presentes.

## Estrutura

Hero com pessoa e produto; rotina do escritório; solução; tour interativo de três telas; processo; comparação de fluxo; público indicado; FAQ; CTA final. O tour permite clique e navegação pelas teclas de seta, Home e End. O FAQ usa `details` nativo.

## Desenvolvimento

```bash
npm install
npm run dev
npm run build
```

O build gera `dist/` para hospedagem estática. Componentes ficam em `src/components/`, conteúdo e FAQ em `src/data/content.ts`, estilos em `src/styles/` e imagens em `public/assets/`.

Defina `PUBLIC_SITE_URL` com a URL real de publicação para canonical/OG. O GTM é opcional: configure `PUBLIC_GTM_ID` apenas após validar a propriedade correta com o responsável. Não foram copiadas IDs de tracking do SMSMais.

## Antes de usar em campanha

- O briefing estratégico ainda está pendente.
- Não foi informado destino confirmado para leads (formulário, CRM, e-mail ou WhatsApp). Por isso os CTAs levam ao site oficial `https://datadom.com.br/`; não há formulário que finja captar contatos.
- As capturas têm dados demonstrativos; a página as identifica como ilustrativas.
- As fotos de pessoas são ilustrativas, não retratam a equipe ou clientes reais da DataDom.
- Validar com o cliente a promessa D-1, uso de screenshots e texto final antes de conectar tráfego.
- A inspeção visual renderizada desta revisão ainda está pendente: o navegador bloqueou a prévia local por sua política de URL. O build, os arquivos e os scripts foram verificados sem contornar essa regra.
