# ASbot - Şikayet & Öneri Sistemi 

🤩 Anadolu Sigorta sponsorluğundaki Hack Series'in ilk Hackathonu kapsamında kullanıcıların sorularına hızlı ve etkili bir şekilde cevap verebilen bir chatbot geliştirdik. Bu chatbot, kullanıcıların anadolu sigorta ürünleri ile ilgili çeşitli konularda bilgi edinmelerine yardımcı olacak şekilde tasarlandı. Ayrıca, kullanıcı deneyimini daha da zenginleştirmek amacıyla, hem uygulama menüsünden hem de chatbot arayüzünden erişilebilen bir şikayet ve öneri sistemi entegre ettik. Bu sistem, kullanıcılara herhangi bir sorunları veya önerileri olduğunda doğrudan geri bildirimde bulunma imkanı sunuyor. Projemizin amacı, kullanıcıların ihtiyaçlarına hızlı ve verimli bir şekilde yanıt vermek ve onlara kapsamlı bir destek sağlamak.

Contributors

[@kubilaygulacdi](https://github.com/kubilaygulacdi) - Data Scientist

[@aydozy](https://github.com/aydozy) - Mobile Developer

## Kullanılan Teknolojiler
- **Web**: Streamlit
- **Mobil**: Dart & Flutter
- **Generative AI**: Langchain, OpenAI
- **Backend**: Python, MongoDB, ChromaDB, Flask

## Asbot - Şikayet & Öneri Gen AI Özellikler

**ChatOpenAI**: OpenAI'nin GPT-3.5 modelini kullanarak sohbet asistanı oluşturmak için ChatOpenAI sınıfı kullanılır.

**OpenAIEmbeddings**: Metinleri gömülü vektörler (embeddings) haline getirmek için OpenAIEmbeddings kullanılır. Bu, metinlerin semantik analizini ve karşılaştırılmasını sağlar.

**TextLoader**: `TextLoader`, belirli bir dosyadan metinleri yüklemek için kullanılır. Bu, sohbet asistanının temel alacağı kaynak metinleri sağlar.

**RecursiveCharacterTextSplitter**: Bu araç, büyük metinleri daha küçük parçalara ayırır. Bu, büyük metinlerin işlenmesini kolaylaştırır ve verimliliği artırır.

**VectorStore**: `ChromaDB`, metin parçalarını vektörler haline getirip bir depoda saklar. Bu, hızlı ve etkili bir şekilde metin araması yapılmasını sağlar.

**RetrievalQA**: `RetrievalQA`, kullanıcıların sorularına yanıt vermek için belirlenen metinler içinden en uygun bilgiyi alır.

**query**: Bu fonksiyon, kullanıcıdan alınan soruları işleyerek uygun yanıtlar üretir. Bu süreçte PromptTemplate ve RetrievalQA kullanılır.

**Template**: Bu, kullanıcının sorularını ve temel alınan metinleri bir araya getirerek soru-cevap sisteminin çalışmasını sağlayan bir format şablonudur.

## Asbot - Şikayet & Öneri Mobil Özellikler

**HTTP GET İsteği**:
- Verilen bir URL'ye HTTP GET isteği gönderir.
- http paketini kullanarak ağ isteklerini gerçekleştirir.
- Asenkron bir işlevdir ve HTTP isteğinin yanıtını bekler.

**ChatScreen Sınıfı**:
- Uygulamanın ana chat ekranını yönetir.
- Kullanıcı mesajlarını yönetmek için `TextEditingController` kullanır.
- Gönderilen ve alınan mesajları liste şeklinde saklar.
- Kullanıcıya başlangıçta varsayılan bir mesaj gösterir.
- Kullanıcıdan gelen mesajları alıp, API aracılığıyla cevaplarını getirir.

**ComplaintPage Sınıfı**:
- Şikayet ve öneri formu için ayrı bir sayfa oluşturur.
- Kullanıcıdan çeşitli bilgiler almak için `TextEditingController` kullanır.
- Tarih seçimi için bir DatePicker entegre edilmiştir.
- Şikayet verisini API'ye göndermek için submitComplaint fonksiyonunu kullanır.

**WelcomeScreen Sınıfı**:
- Uygulamanın karşılama ekranını oluşturur.
- Bir arka plan resmi gösterir (mockup olarak görev alır) ve chat ekranına geçiş için bir buton içerir.

## ASbot Uygulama Görüntüsü

  <img src="https://github.com/kubilaygulacdi/Hackathon-AnadoluSigorta/assets/104395137/7db253d6-3b1b-4f0d-b676-20746047a82a" width="250" height="500">

## Şikayet & Öneri Sistemi Uygulama Görüntüsü

Projemizde, Anadolu Sigorta'nın var olan uygulama tasarımlarına sadık kaldık, böylece marka tutarlılığını koruyarak kullanıcılara tanıdık bir deneyim sunduk. Bu yaklaşım, hem marka kimliğini güçlendirmeyi hem de kullanıcı memnuniyetini artırmayı hedefliyor.

<img src="https://github.com/kubilaygulacdi/Hackathon-AnadoluSigorta/assets/104395137/191c020f-b26d-4a43-8e1b-b295af6e19c0" width="250" height="500">

## ASbot Demo

[![Video Önizleme](https://github.com/kubilaygulacdi/Hackathon-AnadoluSigorta/assets/104395137/your-preview-image.jpg)](https://github.com/kubilaygulacdi/Hackathon-AnadoluSigorta/assets/104395137/ac43619a-863f-4229-bbac-950aece9283f)




