# Sumatera Birds Sound Classification
Telah dilakukan identifikasi suara Burung di Pulau Sumatera dengan menerapkan Transfer Learning pada Deep Neural Network. Adapun Model yang digunakan adalah 
1. Resnet50 
2. VGG-16
3. EfficientNet B4
4. DenseNet169
5. Xception

Data yang digunakan bersumber dari platform XenoCanto yang merupakan platform suara Burung Sedunia, dengan total file audio adalah 2063 file mp3. File audio dibagi 5 detik yang kemudian di ekstrak menjadi gambar Mels Spectrogram sebagai input multiclass pada model Transfer Learning. pembagian data pelatihan, data validasi, dan data test adalah 80:10:10. Selanjutnya digunakan optimisasi loss function sebagai berikut:
1. Adam
2. RMSprop

Hyperparameter
Digunakan droput rate 20% dan 50%, Learning rate 0,0001 dan 0,00001, dan batch size sebesar 16 dan 32 pada model Resnet50 dan Densenet169.
sedangkan pada model VGG-16, EfficientNet B4 dan Xception parameter dijaga pada dropout sebesar 50%, learning rate sebesar 0,0001 dan batch size sebesar 16.

Model
Sebanyak 22 model yang telah dilatih dengan data pelatihan gambar sebanyak 10,590 berkas gambar dan data validasi dan test sebanyak 1.303 berkas gambar

Evaluasi
Digunakan nilai akurasi dan loss, kemudian F1 score dan AUCROC Score pada masing-masing spesies.

13 spesies Burung yang ditemukan di Region Pulau Sumatera dengan kelimpahan data lebih dari 50 file dan kualitas audio paling baik adalah:
1. White-bellied Woodpecker (_Dryocopus javensis_)
2. Large-tailed Nightjar (_Caprimulgus macrurus_)
3. Pygmy Cupwing (_Pnoepyga pusilla_)
4. Rufous-tailed Tailorbird (_Orthotomus sericeus_)
5. Horsfield's Babbler (_Malacocincla sepiaria_)
6. Sooty-capped Babbler (_Malacopteron affine_)
7. Mangrove Whistler (_Pachycephala cinerea_)
8. Slender-billed Crow (_Corvus enca_)
9. Rufous-browed Flycatcher (_Anthipes solitaris_)
10. Black-winged Kite (_Elanus caeruleus_)
11. Oriental Pied Hornbill (_Anthracoceros albirostris_)
12. Arctic Warbler (_Phylloscopus borealis_)
13. Pin-striped Tit-Babbler (_Macronus gularis_)
