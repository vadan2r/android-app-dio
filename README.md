# Esse projeto tem o objetivo de realizar um desafio para os alunos do curso de Android na DIO

# 🌍 Meu Primeiro App - Internacionalização

Este projeto faz parte de um exercício de Android com Kotlin, cujo objetivo é **implementar internacionalização (i18n)** em um aplicativo simples.

## 📌 Objetivo
- Criar uma string no arquivo `strings.xml`.
- Adicionar traduções para diferentes idiomas (Português, Inglês e Espanhol).
- Usar essa string no layout principal (`activity_main.xml`).
- Permitir que o app adapte automaticamente o texto exibido conforme o idioma do dispositivo.

---

## 🧩 Estrutura criada

### Arquivo base (Português)
`res/values/strings.xml`
```xml
<resources>
    <string name="hello_message">Olá, mundo!</string>
</resources>

### Tradução para Inglês
res/values-en/strings.xml

<resources>
    <string name="hello_message">Hello, world!</string>
</resources>


### Tradução para Espanhol
res/values-es/strings.xml

<resources>
    <string name="hello_message">¡Hola, mundo!</string>
</resources>


### 🖼️ Uso no layout
res/layout/activity_main.xml

<TextView
    android:id="@+id/textView"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="@string/hello_message" />


### 🧪 Testes
Para validar a internacionalização:

Instale o app em um dispositivo ou emulador Android.

Vá em Configurações → Idioma e altere para:

🇧🇷 Português → "Olá, mundo!"

🇺🇸 Inglês → "Hello, world!"

🇪🇸 Espanhol → "¡Hola, mundo!"

Abra o app e verifique a mudança automática do texto.

### ✅ Conclusão
O exercício está concluído: o app agora suporta múltiplos idiomas e adapta o texto exibido conforme a configuração de idioma do sistema Android.