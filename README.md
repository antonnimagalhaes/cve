# Comunidade Venda Estratégica

Plataforma completa de comunidade gamificada com app nativo, desenvolvida com Next.js 14, Supabase, Tailwind CSS e Flutter.

## 📋 Visão Geral

A Comunidade Venda Estratégica é uma plataforma completa para comunidades online, com foco em gamificação, engajamento e aprendizado. O sistema inclui:

- Frontend web responsivo em Next.js 14
- Banco de dados Supabase
- UI moderna com Tailwind CSS
- App nativo em Flutter
- PWA com notificações push via OneSignal

## 🚀 Funcionalidades Principais

### 👥 Área de Login e Perfil
- Autenticação via Supabase (e-mail/senha)
- Perfil do aluno com foto, nome, bio, progresso e XP
- Dashboard individual com XP total, missões, trilhas e conquistas

### 📚 Aulas e Certificação
- Área de aulas com vídeos (via Panda Video embed)
- Upload e visualização de materiais PDF
- Progresso de aulas (por usuário)
- Avaliações e quizzes após conclusão
- Emissão automática de certificados
- Trilhas de aprendizado sequenciais

### 🏆 Gamificação Completa
- Sistema de XP por ações (aulas, posts, comentários)
- Ranking individual e por equipes
- Missões semanais com recompensas
- Insígnias por conquistas
- Loja de recompensas para troca de XP

### 📱 Feed e Comunidade
- Feed de conteúdo com curtidas e comentários
- Busca inteligente de conteúdo
- Notificações em tempo real
- Agenda de eventos e lives
- Histórias de Sucesso com depoimentos reais

### 📊 Painel Administrativo
- Moderação de posts, sugestões e comentários
- Métricas de participação, aulas assistidas, posts feitos
- Gráfico de presença em lives e ranking de participação
- Exportação de dados em CSV

### 📱 Aplicativo Nativo
- Criado em Flutter com layout adaptado
- Modo escuro ativado
- Login com Supabase
- Mesmas funcionalidades da versão web
- Push Notifications
- Projeto Flutter pronto para publicação

## 🛠️ Requisitos Técnicos

- Node.js 18+ (recomendado: 20.x)
- NPM 9+
- Flutter 3.10+
- Dart 3.0+
- Conta no Supabase
- Conta no Panda Video (para hospedagem de vídeos)
- Conta no OneSignal (para notificações push)

## ⚙️ Configuração e Instalação

### 1. Clone o repositório
```bash
git clone https://seu-repositorio/comunidade-venda-estrategica.git
cd comunidade-venda-estrategica
```

### 2. Instale as dependências do projeto web
```bash
npm install
```

### 3. Configure as variáveis de ambiente
Crie um arquivo `.env.local` na raiz do projeto baseado no `.env.example` fornecido:

```
NEXT_PUBLIC_SUPABASE_URL=sua_url_do_supabase
NEXT_PUBLIC_SUPABASE_ANON_KEY=sua_chave_anonima_do_supabase
NEXT_PUBLIC_OPENAI_API_KEY=sua_chave_da_openai
NEXT_PUBLIC_PANDAVIDEO_API_KEY=sua_chave_do_pandavideo
NEXT_PUBLIC_ONESIGNAL_KEY=sua_chave_do_onesignal
NEXT_PUBLIC_GOOGLE_CALENDAR_ID=seu_id_do_google_calendar
```

### 4. Execute o projeto web em desenvolvimento
```bash
npm run dev
```

### 5. Configuração do App Flutter
```bash
cd flutter_app
flutter pub get
```

Crie um arquivo `.env` na pasta `flutter_app` com as mesmas variáveis do projeto web.

### 6. Execute o app Flutter
```bash
flutter run
```

### 7. Build para produção (Web)
```bash
npm run build
npm run start
```

### 8. Build do app Flutter para Android
```bash
cd flutter_app
flutter build apk --release
```

O arquivo APK será gerado em `flutter_app/build/app/outputs/flutter-apk/app-release.apk`

## 🗄️ Estrutura do Banco de Dados Supabase

O projeto utiliza as seguintes tabelas no Supabase:

- `profiles`: Perfis de usuários
- `user_xp`: XP dos usuários
- `xp_history`: Histórico de XP
- `posts`: Posts do feed
- `comments`: Comentários nos posts
- `post_likes`: Curtidas nos posts
- `trilhas`: Trilhas de aprendizado
- `aulas`: Aulas das trilhas
- `user_aula_progress`: Progresso dos usuários nas aulas
- `certificados`: Certificados emitidos
- `missions`: Missões disponíveis
- `user_missions`: Missões dos usuários
- `achievements`: Conquistas disponíveis
- `user_achievements`: Conquistas dos usuários
- `rewards`: Recompensas da loja
- `user_rewards`: Recompensas adquiridas pelos usuários
- `lives`: Agenda de lives
- `live_attendance`: Presença em lives
- `notifications`: Notificações dos usuários
- `admin_users`: Usuários administradores

## 📱 Configuração do PWA

O projeto já está configurado como PWA, com:

- Manifesto web
- Service Worker para cache
- Ícones em diferentes tamanhos
- Tela de splash
- Suporte a instalação no dispositivo

## 🔔 Configuração de Notificações Push

1. Crie uma conta no OneSignal (https://onesignal.com)
2. Configure um novo aplicativo web
3. Adicione sua chave do OneSignal no arquivo `.env.local`
4. As notificações push já estão integradas no código

## 📹 Integração com Panda Video

1. Crie uma conta no Panda Video (https://pandavideo.com)
2. Obtenha sua API Key
3. Adicione a chave no arquivo `.env.local`
4. Faça upload dos vídeos no Panda Video
5. Use os IDs dos vídeos nas aulas da plataforma

## 🚀 Deploy na Vercel

O projeto está pronto para deploy na Vercel:

1. Conecte seu repositório à Vercel
2. Configure as variáveis de ambiente
3. Deploy automático a cada push

## 📱 Publicação do App Flutter

### Google Play Store
1. Crie uma conta de desenvolvedor na Google Play Console
2. Gere uma chave de assinatura para o app
3. Configure o app no Google Play Console
4. Faça upload do APK ou Bundle

### Apple App Store
1. Crie uma conta no Apple Developer Program
2. Configure o app no App Store Connect
3. Use o Xcode para gerar o arquivo IPA
4. Faça upload do app usando o Xcode ou Application Loader

## 📄 Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo LICENSE para detalhes.

## 📞 Suporte

Para suporte, entre em contato através do email: suporte@comunidadevendaestrategica.com
