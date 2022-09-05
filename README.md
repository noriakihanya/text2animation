# text2animation
テキストから画像を生成するAI「StableDiffusion」と2つの入力画像から複数の中間フレームを合成するフレーム補間アルゴリズム「FILM: Frame Interpolation for Large Motion」を用いたアニメーション生成プログラム.

* StableDiffusion
https://github.com/CompVis/stable-diffusion
* FILM: Frame Interpolation for Large Motion
https://github.com/google-research/frame-interpolation

# DEMO



# Features


# Requirement
* diffusers
* frame-interpolation
* Real-ESRGAN（画像の高解像度化プログラム）

# Usage
* Access Tokensの取得<br>
1. 初めに、以下のサイトからHuggingFaceのアカウントを作成し、CompVis/stable-diffusion-v1-4へのAccess Tokensを取得<br>
https://huggingface.co<br>
※[Settings]->[Access Tokens]に移動しNewTokenをコピーし、Access Tokenの入力フォームへペースト
<img width="231" alt="スクリーンショット 2022-09-05 16 46 36" src="https://user-images.githubusercontent.com/105255463/188396200-aaa52531-b73e-4301-8f11-ea2c62769876.png">
<img width="855" alt="スクリーンショット 2022-09-05 16 47 42" src="https://user-images.githubusercontent.com/105255463/188396409-4ba60f3c-3942-45b0-b900-965350ece6f0.png">

* FILMの学習済みモデルのロード
FILMのモデルはColabからダウンロードできないため、GoogleDriveのMyDriveにモデルのショートカットを追加しロードできるようにする。

* promptの入力
<img width="1105" alt="スクリーンショット 2022-09-05 16 43 16" src="https://user-images.githubusercontent.com/105255463/188395581-b7bc3574-493c-4dc7-94a1-9ee13d3c40d4.png">

* アニメーションの再生時間を入力
<img width="548" alt="スクリーンショット 2022-09-05 16 44 57" src="https://user-images.githubusercontent.com/105255463/188395865-a7c0aaff-4b98-4a78-a36e-0c3da1f67e3d.png">

