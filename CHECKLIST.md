# Checklist de Implantação - Comunidade Venda Estratégica

Este documento contém o passo a passo para configurar e publicar sua Comunidade Venda Estratégica. Siga as instruções abaixo para ter sua plataforma funcionando rapidamente.

## 1. Configuração do Supabase

- [ ] Criar conta no Supabase (https://supabase.com)
- [ ] Criar novo projeto
- [ ] Copiar URL do projeto e chave anônima
- [ ] Executar script SQL de criação de tabelas (disponível na pasta `/database/schema.sql`)
- [ ] Configurar autenticação por e-mail/senha
- [ ] Configurar políticas de segurança (RLS)

## 2. Configuração das APIs Externas

- [ ] Criar conta no OpenAI (https://openai.com)
  - [ ] Gerar API Key para o módulo "IA Professor"
  
- [ ] Criar conta no Panda Video (https://pandavideo.com)
  - [ ] Gerar API Key para hospedagem de vídeos
  - [ ] Fazer upload dos vídeos das aulas
  
- [ ] Criar conta no OneSignal (https://onesignal.com)
  - [ ] Configurar novo aplicativo web
  - [ ] Configurar novo aplicativo Android/iOS
  - [ ] Obter App ID e API Key
  
- [ ] Configurar Google Calendar (opcional)
  - [ ] Criar calendário para eventos e lives
  - [ ] Obter ID do calendário e API Key

## 3. Configuração do Projeto Web

- [ ] Copiar arquivo `.env.example` para `.env.local`
- [ ] Preencher todas as variáveis de ambiente no `.env.local`
- [ ] Personalizar cores e logotipo (em `/public/images/`)
- [ ] Personalizar textos e conteúdo inicial (em `/data/`)
- [ ] Testar localmente com `npm run dev`

## 4. Deploy do Projeto Web

- [ ] Criar conta na Vercel (https://vercel.com)
- [ ] Conectar repositório Git
- [ ] Configurar variáveis de ambiente na Vercel
- [ ] Realizar deploy
- [ ] Configurar domínio personalizado (opcional)

## 5. Configuração do App Flutter

- [ ] Copiar arquivo `.env.example` para `.env` na pasta `flutter_app`
- [ ] Preencher todas as variáveis de ambiente
- [ ] Personalizar ícones e splash screen (em `/flutter_app/assets/`)
- [ ] Testar localmente com `flutter run`

## 6. Publicação do App Flutter

- [ ] Criar conta de desenvolvedor na Google Play Console
- [ ] Configurar app no Google Play Console
- [ ] Gerar chave de assinatura para o app
- [ ] Compilar APK/Bundle com `flutter build appbundle --release`
- [ ] Fazer upload do app para a Google Play Store
- [ ] Configurar conta de desenvolvedor na Apple (opcional)
- [ ] Publicar na App Store (opcional)

## 7. Configuração do PWA

- [ ] Verificar manifesto web em `/public/manifest.json`
- [ ] Personalizar ícones PWA em `/public/icons/`
- [ ] Testar instalação do PWA no navegador

## 8. Pós-Implantação

- [ ] Criar usuário administrador
- [ ] Configurar trilhas de aprendizado
- [ ] Adicionar aulas iniciais
- [ ] Configurar missões e conquistas
- [ ] Testar emissão de certificados
- [ ] Verificar notificações push
- [ ] Testar integração com IA Professor

## Contatos para Suporte

Em caso de dúvidas ou problemas durante a implantação, entre em contato:

- Suporte Técnico: suporte@vendaestrategica.com.br
- WhatsApp: +55 (XX) XXXXX-XXXX
