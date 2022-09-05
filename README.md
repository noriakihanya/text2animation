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
・初めに、以下のサイトからHuggingFaceのアカウントを作成し、CompVis/stable-diffusion-v1-4へのにAccess Tokensを取得
・[Settings]->[Access Tokens]に移動しNewTokenをコピーし、Access Tokenの入力フォームへペースト

https://huggingface.co

参考サイト
https://www.12-technology.com/2022/08/stable-diffusion-aipython.html
