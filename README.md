# Landing Page Moderna

Uma landing page moderna, responsiva e animada construída com React, Tailwind CSS e Framer Motion.

## 🎯 Características

- **Design Responsivo** - Funciona perfeitamente em dispositivos móveis, tablets e desktops
- **Animações Suaves** - Transições elegantes com Framer Motion
- **Menu Mobile** - Navegação intuitiva para dispositivos móveis
- **Seções Completas**:
  - Hero com CTA (Call-to-Action)
  - Recursos principais
  - Depoimentos de clientes
  - Seção de preços
  - Footer com links
- **Dark Theme** - Tema escuro moderno com cores vibrantes
- **Performance** - Otimizada para velocidade e SEO

## 🛠 Tecnologias Utilizadas

- **React** - Biblioteca JavaScript para construção de UIs
- **Tailwind CSS** - Framework CSS utilitário para estilos
- **Framer Motion** - Biblioteca para animações em React
- **Lucide React** - Ícones SVG de alta qualidade
- **Vite** - Build tool rápido e moderno

## 📦 Instalação

### Pré-requisitos
- Node.js 16+ instalado
- npm ou yarn

### Passos

1. Clone o repositório:
```bash
git clone <seu-repositorio>
cd <nome-do-projeto>
```

2. Instale as dependências:
```bash
npm install
```

3. Inicie o servidor de desenvolvimento:
```bash
npm run dev
```

4. Abra o navegador e acesse:
```
http://localhost:5173
```

## 🚀 Como Usar

### Estrutura do Projeto

```
src/
├── App.jsx          # Componente principal
├── App.css          # Estilos globais
└── index.css        # Configuração Tailwind
```

### Personalizando o Conteúdo

#### Logo/Marca
Encontre e substitua `"Minha marca"` por seu nome de marca:
```jsx
<span className='font-bold tracking-tight'>Sua Marca Aqui</span>
```

#### Hero Section
Altere o título e descrição:
```jsx
<h1>Seu título aqui</h1>
<p>Sua descrição aqui</p>
```

#### Recursos
Modifique o array de features com seus próprios recursos:
```jsx
{
  title: "Seu Recurso",
  desc: "Descrição do recurso",
  icon: <SeuIcone className='size-5' />
}
```

#### Preços
Atualize o valor e benefícios:
```jsx
<div className='text-5xl font-extrabold mt-2'>R$ Seu Valor</div>
```

#### Depoimentos
Customize com depoimentos reais:
```jsx
<p className='mt-3 text-slate-300'>Seu depoimento aqui</p>
<footer className='mt-3 text-sm text-slate-400'>- Nome do Cliente</footer>
```

#### Links de Navegação
Atualize o array `navLinks` no topo do arquivo:
```jsx
const navLinks = [
  { href: "#features", label: "Recursos" },
  { href: "#testimonials", label: "Depoimentos" },
  { href: "#pricing", label: "Preços" },
  { href: "#faq", label: "FAQ" },
];
```

## 🎨 Cores e Temas

O projeto usa Tailwind CSS com as seguintes cores principais:

- **Fundo**: `bg-slate-950` (quase preto)
- **Texto**: `text-slate-100` (branco claro)
- **Primária**: `fuchsia-400/600` (rosa/magenta)
- **Secundária**: `violet-300` (violeta)
- **Destaque 1**: `emerald-400` (verde)
- **Destaque 2**: `sky-400` (azul)
- **Destaque 3**: `amber-400` (âmbar)

Para alterar o tema, modifique as classes Tailwind em todo o arquivo.

## 📱 Responsividade

O projeto utiliza breakpoints do Tailwind:
- `hidden md:flex` - Oculto em mobile, visível em desktop
- `md:grid-cols-2` - 1 coluna em mobile, 2 em desktop
- `lg:grid-cols-3` - 3 colunas em telas grandes

## ✨ Animações

As animações são controladas por Framer Motion:

```jsx
<motion.h1
  initial={{ opacity: 0, y: 20 }}      // Estado inicial
  animate={{ opacity: 1, y: 0 }}       // Estado final
  transition={{ duration: 1, delay: 0.5 }} // Configuração
>
  Conteúdo
</motion.h1>
```

Você pode ajustar:
- `duration` - Duração da animação em segundos
- `delay` - Atraso antes da animação começar
- `initial` - Propriedades iniciais
- `animate` - Propriedades finais

## 🔧 Scripts Disponíveis

```bash
# Inicia o servidor de desenvolvimento
npm run dev

# Faz build para produção
npm run build

# Visualiza o build de produção localmente
npm run preview

# Lint e verifica código (se configurado)
npm run lint
```

## 📦 Dependências Principais

```json
{
  "react": "^18.2.0",
  "framer-motion": "^10.x.x",
  "lucide-react": "^0.x.x"
}
```

## 🚀 Deploy

### Deploy no Vercel (Recomendado)

1. Faça push do código para GitHub
2. Acesse [vercel.com](https://vercel.com)
3. Conecte seu repositório GitHub
4. Clique em "Deploy"
5. Pronto! Seu site estará online

### Deploy no Netlify

1. Faça build do projeto:
```bash
npm run build
```

2. Acesse [netlify.com](https://netlify.com)
3. Arraste a pasta `dist` para deploy
4. Ou conecte seu repositório GitHub para deploy automático

### Deploy em Servidor Próprio

1. Faça build:
```bash
npm run build
```

2. Copie o conteúdo da pasta `dist` para seu servidor
3. Configure seu servidor web (Nginx, Apache, etc.)

## 🐛 Troubleshooting

### Problema: Ícones não aparecem
**Solução**: Certifique-se de que `lucide-react` está instalado:
```bash
npm install lucide-react
```

### Problema: Estilos não aplicados
**Solução**: Verifique se o Tailwind CSS está configurado em `tailwind.config.js`

### Problema: Animações não funcionam
**Solução**: Instale Framer Motion:
```bash
npm install framer-motion
```

## 📄 Licença

Este projeto está disponível sob a licença MIT. Sinta-se livre para usá-lo em projetos pessoais e comerciais.

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para:
1. Fazer fork do projeto
2. Criar uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abrir um Pull Request

## 📞 Suporte

Se tiver dúvidas ou encontrar problemas:
- Abra uma issue no GitHub
- Consulte a documentação do Tailwind: [tailwindcss.com](https://tailwindcss.com)
- Consulte a documentação do Framer Motion: [framer.com/motion](https://www.framer.com/motion)

## 🎓 Aprenda Mais

- [React Documentation](https://react.dev)
- [Tailwind CSS](https://tailwindcss.com)
- [Framer Motion](https://www.framer.com/motion)
- [Lucide Icons](https://lucide.dev)

---

**Desenvolvido com ❤️ usando React, Tailwind CSS e Framer Motion**
