### 📦 Shared — object-of-values
- Este diretório contém componentes compartilhados essenciais para a implementação de Objetos de Valor (Value Objects) em projetos baseados em Domain-Driven Design (DDD). Ele oferece abstrações reutilizáveis que facilitam a criação de Value Objects consistentes e fáceis de manter.

#### 🔧 Estrutura do Diretório
- A estrutura atual do diretório shared é a seguinte:

```
shared/
├── interfaces/
│   └── value-object.interface.ts
└── utils/
    └── value-object.util.ts

```
- interfaces/: Contém interfaces que definem contratos para os Value Objects, promovendo consistência e reutilização de código.
- utils/: Inclui utilitários auxiliares que facilitam operações comuns com Value Objects, como comparação e validação.

#### ⚙️ Objetivo

- O objetivo deste diretório é fornecer ferramentas que:
- Definam contratos claros para Value Objects, garantindo consistência em toda a aplicação.
- Facilitem a implementação de Value Objects, oferecendo abstrações reutilizáveis.
- Promovam boas práticas de DDD, como imutabilidade e comparação baseada em valor.

### 📘 Exemplo de Uso
- Criando um Value Object

```
import { ValueObjectUtil } from './utils/value-object.util';

const email1 = new Email('exemplo@dominio.com');
const email2 = new Email('exemplo@dominio.com');

const saoIguais = ValueObjectUtil.equals(email1, email2);

```

#### 📚 Contribuindo

- Contribuições são bem-vindas! Para contribuir:
- Faça um fork deste repositório.
- Crie uma branch para sua feature (git checkout -b minha-feature).
- Faça commit das suas alterações (git commit -am 'Adiciona nova feature').
- Envie para o repositório remoto (git push origin minha-feature).
- Abra um Pull Request.

#### 📄 Licença
- Este projeto está licenciado sob a MIT License.
