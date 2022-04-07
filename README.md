# ما هي مراحل Transformers؟
لتقرأ السطور القليلة القادمة فأنا افترض ان لديك معرفة ب NN , RNN ,Transformers 
## المرحلة الاولى Embedding the inputs
وفي هذه المرحلة يتم عرض مجموعة من unstrctured text data على الموديل حتى لا يبدأ من الصفر عند التدريب 
## المرحلة الثانية The Positional Encodings
وهي تحديد موضع كل كلمة وتحديد مكانها وعلاقتها بالكلمات الاخرى في الجملة ومعنى كل كلمة 
## المرحلة التالته Creating Masks
وهي مهمه جدا في العملية سواء في encoder and decoder: To zero attention outputs wherever there is just padding in the input sentences
وفي decoder عشان يمنع peaking
## المرحلة الرابعة The Multi-Head Attention layer
دي مرحلةة layers في الشبكة العصبية 
## المرحلة الخامسه The Feed-Forward layer 
ودي بستخدم فيها Relu كــــــactivation function
![alt text](1_2vyKzFlzIHfSmOU_lnQE4A.png)
