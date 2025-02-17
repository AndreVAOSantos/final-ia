por conta dessa indicação do transformers aparece essa mensagem semelhante a um erro :

"D:\python\Lib\site-packages\transformers\models\whisper\generation_whisper.py:573: FutureWarning: The input name `inputs` is deprecated. Please make sure to use `input_features` instead.
  warnings.warn(
Due to a bug fix in https://github.com/huggingface/transformers/pull/28687 transcription using a multilingual Whisper will default to language detection followed by transcription instead of translation to English.This might be a breaking change for your use case. If you want to instead always translate your audio to English, make sure to pass `language='en'`.
Passing a tuple of `past_key_values` is deprecated and will be removed in Transformers v4.43.0. You should pass an instance of `EncoderDecoderCache` instead, e.g. `past_key_values=EncoderDecoderCache.from_legacy_cache(past_key_values)`."
 

porém o programa executa normalmente apenas sendo nescessário falar pausadamente para que o programa identifique os numeros.

versão do python utilizada:3.12.4

primeiro comando antes de executar:
baixar requirements.txt
py -m pip install -r requirements.txt

após baixar, execute o seguinte comando:
baixe e punkt_tab do NLTK
py -m nltk.downloader punkt_tab

Finalmente execute o arquivo assistente.py
foi ultilizado o openai wispers imbutido no codigo
