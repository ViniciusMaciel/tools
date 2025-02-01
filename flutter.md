# Configuração do Ambiente Flutter no VS Code

## 🖥️ Configuração para Windows

### ✅ 1. Instalar o VS Code
- Baixe e instale o **VS Code**:  
  🔗 [Download VS Code](https://code.visualstudio.com/)

### ✅ 2. Instalar o Flutter e Dart
1. Baixe o Flutter SDK:  
   🔗 [Flutter para Windows](https://docs.flutter.dev/get-started/install/windows)
2. Extraia o arquivo ZIP para `C:\flutter` (ou outro local de sua escolha).
3. Adicione `C:\flutter\bin` ao **PATH** do Windows:
   - Abra o **Painel de Controle** → **Sistema** → **Configurações Avançadas do Sistema** → **Variáveis de Ambiente**.
   - Em **Variáveis do Sistema**, encontre `Path`, clique em **Editar** e adicione `C:\flutter\bin`.
4. Reinicie o computador para aplicar as mudanças.

### ✅ 3. Instalar o SDK do Android (Para rodar no Emulador ou Celular)
1. Baixe e instale o **Android Studio**:  
   🔗 [Download Android Studio](https://developer.android.com/studio)
2. Abra o Android Studio e vá em **Configurações** → **SDK Manager** → Baixe o **Android SDK**.
3. Para rodar no **Emulador**, crie um **AVD (Android Virtual Device)** no **AVD Manager**.
4. Para rodar no **celular físico**, ative o **Modo Desenvolvedor** e **Depuração USB** no Android.

### ✅ 4. Instalar Extensões no VS Code
- Abra o **VS Code** e vá até **Extensões (Ctrl + Shift + X)**.
- Instale as extensões:
  - ✅ **Flutter**
  - ✅ **Dart**

### ✅ 5. Verificar a Instalação
Abra o **Prompt de Comando (cmd)** ou **PowerShell** e execute:
```bash
flutter doctor
```
Se houver problemas, o comando mostrará o que falta configurar.

### ✅ 6. Criar e Rodar um Projeto Flutter
```bash
flutter create my_app
cd my_app
flutter run
```
Isso iniciará o app no emulador ou no celular conectado.

---

## 🍏 Configuração para macOS

### ✅ 1. Instalar o VS Code
- Baixe e instale o **VS Code**:  
  🔗 [Download VS Code](https://code.visualstudio.com/)

### ✅ 2. Instalar o Flutter e Dart
1. Baixe o Flutter SDK:  
   🔗 [Flutter para macOS](https://docs.flutter.dev/get-started/install/macos)
2. Extraia os arquivos e mova para um local fixo, ex: `/Users/seu_usuario/flutter`.
3. Adicione `flutter/bin` ao **PATH** do sistema:
   - Abra o **Terminal** e edite o arquivo `.zshrc` ou `.bashrc` com:
     ```bash
     export PATH="$PATH:/Users/seu_usuario/flutter/bin"
     ```  
   - Salve e execute:
     ```bash
     source ~/.zshrc  # ou source ~/.bashrc
     ```

### ✅ 3. Instalar o Xcode (Para rodar no iOS)
1. Baixe e instale o **Xcode** pela Mac App Store.
2. Instale as dependências:
   ```bash
   sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer
   sudo gem install cocoapods
   ```

### ✅ 4. Instalar o SDK do Android (Para rodar no Emulador ou Celular Android)
1. Baixe e instale o **Android Studio**:  
   🔗 [Download Android Studio](https://developer.android.com/studio)
2. No **SDK Manager**, baixe o **Android SDK**.
3. No **AVD Manager**, crie um **Emulador Android**.
4. Para rodar no **celular físico**, ative o **Modo Desenvolvedor** e **Depuração USB** no Android.

### ✅ 5. Instalar Extensões no VS Code
- No VS Code, vá até **Extensões (Cmd + Shift + X)**.
- Instale as extensões:
  - ✅ **Flutter**
  - ✅ **Dart**

### ✅ 6. Verificar a Instalação
Abra o **Terminal** e execute:
```bash
flutter doctor
```
Se houver problemas, o comando mostrará o que falta configurar.

### ✅ 7. Criar e Rodar um Projeto Flutter
```bash
flutter create my_app
cd my_app
flutter run
```
Se quiser rodar no **simulador do iPhone**, execute:
```bash
open -a Simulator
flutter run
```
