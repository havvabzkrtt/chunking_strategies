# CHUNKING STRATEJİLERİ

Chunking stratejileri, büyük metin bloklarını daha küçük, yönetilebilir parçalara bölme yöntemleridir. Bu stratejiler, metnin türüne, yapısına ve analiz amacına göre değişiklik gösterebilir.

## RecursiveCharacterTextSplitter.ipynb

- `RecursiveCharacterTextSplitter` ile text değişkenindeki 3 paragraflık yazı ve PDF.pdf dosyası parçalandı.

## NLTKTextSplitter.ipynb

- `NLTKTextSplitter` ile text değişkenindeki 3 paragraflık yazı ve PDF.pdf dosyası parçalandı.
- NLTK (The Natural Language Toolkit), Python için sembolik ve istatistiksel doğal dil işleme (NLP) kütüphanesidir.
- Metin, NLTK tokenizer ile bölünür ve chunk boyutu karakter sayısına göre ölçülür.

## SpacyTextSplitter.ipynb

- `SpacyTextSplitter` ile text değişkenindeki 3 paragraflık yazı ve PDF.pdf dosyası parçalandı.
- spaCy, Python ve Cython dillerinde yazılmış gelişmiş doğal dil işleme kütüphanesidir.
- Metin, spaCy tokenizer ile bölünür ve chunk boyutu karakter sayısına göre ölçülür.

## LatexTextSplitter.ipynb

- `LatexTextSplitter` ile text değişkenindeki 3 paragraflık yazı ve PDF.pdf dosyası parçalandı.
- LaTeX, akademik makaleler ve teknik belgeler için kullanılan bir belge hazırlama sistemi ve biçimlendirme dilidir.
- LaTeX komutlarını ve ortamlarını ayrıştırarak içerik türüne uygun parçalar oluşturur.

## MarkdownTextSplitter.ipynb

- `MarkdownTextSplitter` ile text değişkenindeki 3 paragraflık yazı ve PDF.pdf dosyası parçalandı.
- **Content-Aware Splitting**: Markdown, LaTeX, HTML gibi yapılandırılmış belgelerde içerik türüne ve yapısına odaklanır.

## semantic_chunker.ipynb

- Semantic chunker, gömme benzerliğini kullanarak cümleler arasındaki kesme noktalarını belirler.
- PDF.pdf ve fransa.txt dosyalarındaki veriler parçalandı.
    - `splitter`: 49 chunk
    - `base_splitter`: 116 chunk
    - `parser`: 44 chunk
- `splitter`, `base_splitter` ve `parser` farklı metin bölme stratejilerini uygular.
    - `buffer_size=1`: Her düğümü bağımsız olarak işler.
    - `breakpoint_percentile_threshold=95`: Gömüm mesafesinin 95. persentilini aşan kesme noktalarını belirler.
    - `embed_model=embed_model`: Gömüm modelini kullanarak anlamsal kopmaları belirler.
