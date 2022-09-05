# text2animation
テキストから画像を生成するAI「StableDiffusion」と2つの入力画像から複数の中間フレームを合成するフレーム補間アルゴリズム「FILM: Frame Interpolation for Large Motion」を用いたアニメーション生成プログラム.

* StableDiffusion
https://github.com/CompVis/stable-diffusion
* FILM: Frame Interpolation for Large Motion
https://github.com/google-research/frame-interpolation

# DEMO



# Requirement
* diffusers
* frame-interpolation
* Real-ESRGAN（画像の高解像度化プログラム）

# Usage
* Access Tokensの取得<br>
以下のサイトからHuggingFaceのアカウントを作成し、CompVis/stable-diffusion-v1-4へのAccess Tokensを取得<br>
https://huggingface.co<br>
※[Settings]->[Access Tokens]に移動しNewTokenをコピーし、Access Tokenの入力フォームへペースト
<img width="231" alt="スクリーンショット 2022-09-05 16 46 36" src="https://user-images.githubusercontent.com/105255463/188396200-aaa52531-b73e-4301-8f11-ea2c62769876.png">
<img width="855" alt="スクリーンショット 2022-09-05 16 47 42" src="https://user-images.githubusercontent.com/105255463/188396409-4ba60f3c-3942-45b0-b900-965350ece6f0.png">

* Access Tokensの入力
<img width="662" alt="スクリーンショット 2022-09-05 16 50 47" src="https://user-images.githubusercontent.com/105255463/188396987-b91a1e2a-05d7-4a99-9df1-78904ff9b076.png">

* FILMの学習済みモデルのロード
FILMのモデルはColabからダウンロードできないため、GoogleDriveのMyDriveにモデルのショートカットを追加しロードできるようにする。
<img width="903" alt="スクリーンショット 2022-09-02 15 23 41" src="https://user-images.githubusercontent.com/105255463/188397188-0f8661a7-1840-4b47-aa04-4d9514bbe214.png">
<img width="884" alt="スクリーンショット 2022-09-02 15 24 07" src="https://user-images.githubusercontent.com/105255463/188397227-6736fefd-b653-4529-ae08-7f2cfc1ea3d1.png">


* promptの入力
日本語入力に対応しているため、'日本語入力'か'英語入力'を選択する<br>
英語入力にはあらかじめいくつか選択肢を用意しているが、任意の文字列を入力することも可能<br>
<img width="1105" alt="スクリーンショット 2022-09-05 16 43 16" src="https://user-images.githubusercontent.com/105255463/188395581-b7bc3574-493c-4dc7-94a1-9ee13d3c40d4.png">

* アニメーションの再生時間を入力
<img width="548" alt="スクリーンショット 2022-09-05 16 44 57" src="https://user-images.githubusercontent.com/105255463/188395865-a7c0aaff-4b98-4a78-a36e-0c3da1f67e3d.png">

