Stream e ParallelStrem
As diferenças entre o Stream e ParallelStrem basicamente está em seu processamento, o Stream utiliza apenas uma thread para processar, já o ParallelStrem utiliza várias threads.
Um exemplo entre as diferenças são, quando processo uma lista utilizando utilizando Stream, ela fará este processamento único. Já no ParallelStrem ao processar uma lista ele irá dividar ela em sublistas e processar em paralelo.

Nem sempre utilizar o ParallelStrem pensando em processamentos rápidos será uma boa idéia, pois como ele irá criar várias threads de processamento, talvez a máquina que estiver utilizando pode não tera performance esperada se la tiver apenas um núcleo de processamento. Então neste cenário seria melhor a utilização do Stream.
