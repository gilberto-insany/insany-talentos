# Insany — Banco de talentos

Página pública de cadastro de talentos da Insany, com fundo preto, identidade da marca e formulário integrado ao Notion.

**Site:** https://insany-talentos.insany-team-1573.chatgpt.site/

## Executar localmente

O projeto usa HTML e CSS e não exige instalação de dependências nem etapa de build.

```sh
python3 -m http.server 8080
```

Abra http://localhost:8080.

## Estrutura

- `index.html`: página, estilos responsivos e incorporação do formulário.
- `assets/insany-logo.svg`: logo oficial obtido do site da Insany.

## Formulário e respostas

O formulário é hospedado no Notion e incorporado por iframe. Ao enviar, o cadastro entra diretamente na base privada de talentos. Este repositório contém a página pública; os registros dos candidatos permanecem no Notion.

Campos coletados: nome, email, telefone, senioridade, tempo de experiência, disponibilidade, portfólio, LinkedIn, inglês, habilidades e breve descrição.

A confirmação é configurada no editor do formulário do Notion, em **Submit screen**:

- Título: **Obrigado! Seu cadastro foi enviado.**
- Mensagem: **Recebemos suas informações com sucesso e seu perfil já faz parte do banco de talentos da Insany. Vamos conhecer seu trabalho e entraremos em contato quando surgir uma oportunidade alinhada à sua experiência. Obrigado pelo interesse em construir com a gente!**
- **Email me a copy:** desativado.

Para trocar o formulário, atualize o endereço do iframe e o link alternativo em `index.html`. A apresentação escura do formulário usa um filtro CSS aplicado ao iframe.

## Publicação

Publique a raiz deste repositório em uma hospedagem de arquivos estáticos. O endereço do site acima corresponde à publicação atual no Sites; alterações feitas neste repositório não são implantadas automaticamente nessa publicação.

A marca e o logo pertencem à Insany.
