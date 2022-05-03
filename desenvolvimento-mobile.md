# Desenvolvimento de Applicações Mobile :phone: - 03/04/2022

## Preparação do Ambiente de Desenvolvimento

- JDK
- Android SDK
- IDE : [Android Studio](https://developer.android.com/studio)
  - SDK Manager = gerenciamento de pacotes, ferramentas APIS e componentes
  - AVD Manager = possibilidade de emuladores através de dispositivos virtuais


## Estrutura de Projeto Android

- Manifest
  - `<application>`
    - `allowBackup`
    - `icon`
    - `label`
    - `roundIcon`
    - `supportsRtl`
    - `theme`
  - `<activity>` = tela (tem um xml associado a estrutura da tela principal)
    - `name`
    - `exported`
  - `<intent-filter>`
    - `<action>`
    - `<category>` 
- Java = código Fonte
  - Package
    - MainActivity
  - Package Test de instrumentação (tela)
    - test
  - Package Test unitário
    - test
- res (resources) = imagens, ícones, shapes, estilos, strings*(internacionalização do app configurando as strings)
  - Package: drawable
    - xml
  - Layout
    - xml (pallete , design)
  - mipmap
    - icons
  - values
    - colors.xml
    - text.xml (string)- inclui versão pt-BR
- Scripts de Build e Gestão de Dependências
  - buil.gradle
    - Project (plugin , tasks) = configurações globais
    - App level (Module) = sdk, applicationId, dependências

### REFERÊNCIAS

[Conheça o Android Studio Google](https://developer.android.com/studio/intro?hl=pt-br)

[Android Google Developer Cursos](https://developer.android.com/courses?gclid=Cj0KCQjwpcOTBhCZARIsAEAYLuWNjm1t3m3G4g-Mdy3Ua_Qda5iERuUEUbDqj4ujdIJOFLTmQmjf_mkaAhNkEALw_wcB)