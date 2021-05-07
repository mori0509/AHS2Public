# AutoHealthSurvey
Reports your health to your work or school automatically via Microsoft Forms.
Formsを勝手に提出してくれるやつ

## Usage
1. Fork this repository.
1. Ensure GitHub Actions is enabled on the repository.
1. Edit `config.yaml` file with your answers and the URL of the form.
1. Edit `.github/workflows/node.yml` to set when to run.
1. Set your Microsoft (365) account email to `MICROSOFT_EMAIL`, your password to `MICROSOFT_PASSWORD` secrets.
1. Done!

## 使い方
1. このリポジトリをForkボタン(PCでは右上)からForkする スマホは知らん
2. `config.yaml` は編集しなくてよろしい
3. `.github/workflows/node.yml` の6行目で提出時間を決める
4. このリポジトリのSettingsのSecretsでNew repository secretをクリックして`MICROSOFT_EMAIL` にメアド，`MICROSOFT_PASSWORD` にパスワード，`FORMS_URL` にFormsのURLをセット
5. 以上

## Troubleshooting
If the timeout error occurs at clearing Local Storage, try to use virtual or real X display with headful mode.
```console
$ CHROMIUM_HEADFUL=1 npm start
```
