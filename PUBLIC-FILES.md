# Публичные файлы IQOSMod

Подготовленный набор: 10 файлов репозитория, 6 assets стабильного Release и 4 assets диагностического prerelease. Никакие другие рабочие файлы не относятся к публикации.

## Репозиторий main

```text
.gitignore
LICENSES/Harmony-LICENSE.txt
LICENSES/Mono.Cecil-LICENSE.txt
LICENSES/THIRD-PARTY-NOTICES.txt
PRIVACY-AUDIT.ru.md
PUBLIC-FILES.md
README.md
README.ru.md
TEST-PLAN.ru.md
release-public.xml
```

## Release v3.0.6, stable, prerelease=false

```text
IQOSMod_3.0.6_Windows_Public.zip
SHA256SUMS.txt
iqosmod-stable.manifest.json
iqosmod-stable.manifest.sig
iqosmod-stable.zip
release-public.xml
```

## Release v3.0.7-test.1, testing, prerelease=true

```text
SHA256SUMS.txt
iqosmod-testing.manifest.json
iqosmod-testing.manifest.sig
iqosmod-testing.zip
```

## Клиентский ZIP v3.0.6

```text
Mods/00_IQOSBootstrap/0Harmony.dll
Mods/00_IQOSBootstrap/Harmony-LICENSE.txt
Mods/00_IQOSBootstrap/IQOSBootstrap.dll
Mods/00_IQOSBootstrap/ModInfo.xml
Mods/00_IQOSBootstrap/Mono.Cecil-LICENSE.txt
Mods/00_IQOSBootstrap/Mono.Cecil.dll
Mods/00_IQOSBootstrap/THIRD-PARTY-NOTICES.txt
Mods/IQOSMod/IQOSRuntimeGate.dll
Mods/IQOSMod/ModInfo.xml
PRIVACY-AUDIT.ru.md
PUBLIC-FILES.md
README.md
README.ru.md
release-public.xml
```

## Подписанный начальный пакет 17 файлов

```text
Code/Config/IQOSRouletteSettings.txt
Code/IQOSMod.dll
Data/Config/IQOSRouletteSettings.txt
Data/Config/Localization.csv
Data/Config/buffs.xml
Data/Config/items.xml
Data/Config/recipes.xml
Data/ModInfo.xml
Data/Resources/iqosmod_models.unity3d
Data/Resources/iqosmod_vapor.unity3d
Data/UIAtlases/ItemIconAtlas/iqosDeviceIcon.png
Data/UIAtlases/ItemIconAtlas/iqosHeetsIcon.png
Data/UIAtlases/UIAtlas/iqosCraving.png
Data/UIAtlases/UIAtlas/iqosOverdose.png
Data/UIAtlases/UIAtlas/iqosRecovery.png
Data/UIAtlases/UIAtlas/iqosRush.png
Data/UIAtlases/UIAtlas/iqosWithdrawal.png
```

В testing-пакете также 17 файлов: отличается только Code/IQOSMod.dll одной диагностической строкой и Data/ModInfo.xml номером версии. Встроенные Bootstrap manifest/signature/archive совпадают с assets начального stable-пакета. Публичный ключ во всех местах одинаковый.

Локальная фикстура 3.0.8 с намеренной ошибкой не публикуется. Приватный ключ, внутренние Source/Tests/Private, игровые данные/логи и старые непубличные архивы не загружаются.

0Harmony содержит штатные native-helper ресурсы Linux/macOS, таблицу строк и ILRepack.List; они унаследованы из проверенной очищенной зависимости. Клиентский ZIP включает MIT-лицензии и THIRD-PARTY-NOTICES.
