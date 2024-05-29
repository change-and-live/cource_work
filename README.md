# cource_work
Курсовая программа по дисциплине "Технологии программирования", выполненная Киселевой Александрой и Акулининым Андреем
Тема курсовой работы - голосовой ассистент⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
После 2-летнего обучения в нашей ВУЗе, мы поняли, что ни разу не работали с аудио-контентом. Поэтому решили создать голосового ассистента. Ему, а точнее, ей еще много не достает.
Она медлительна и функционал недостаточно велик. Но мы довольны проделанной работой. Мы узнали, как в принципе происходит работа со звуком, начились использовать (и, в первую очередь, узнали) о существовании некоторых библиотек. Также, мы впервые постарались писать код грамотно. С пояснениями, где это нужно, без лишних действий или громоздких (а, иногда, и ненужных) функций.
Есть огромное поле для расширение возможностей нашей Марии (например, подключение спец. библиотеки для офлайн-перевода). Рассматривается также обучение ее с помощьюе машинного обучения (для прогнозирования ответов) или использование нейросети. 
Далее приведен небольшой отрывок, который является первым комментарием в нашей программе.
⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⠀⠐⠲⣶⣶⣶⣆⠀⠀⠀⠀ ⠀⢀⣶⣶⣶⡶⠒⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀     
            ⠀⠀⠀⠀⠀⠀⣿⢻⣿⣿⡆⠀⠀⠀⠀⣼⢹⣿⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀      
            ⠀⠀⠀⠀⠀⣿⠈⢿⣿⣿⡄⠀⠀⣸⠃⢸⣿⣿⡇⠀⠀⠀⣠⡶⠒⠲⣶⣦⡀⠐⢶⣶⣶⡤⠶⣶⣶⣄   ⠒⣶⣶⡶⠂⠐⣶⣶⡶⠂   ⢀⣴⣶⠶⠒⢶⣶⣶⠂⠀⠀⠀⠀
            ⠀⠀⠀⠀⣿⠀⠈⣿⣿⣿⡀⢠⠇⠀⢸⣿⣿⡇⠀⠀⠐⣿⣿⠀⠀⣿⣿⡇⠀⠀⢸⣿⣿⠁⠀⠘⣿⣿⡆⠀  ⣿⣿⡇⠀⣠⣿⣿⡇⠀  ⠀⢿⣿⣿⠀⠀⢸⣿⣿⠀⠀⠀⠀⠀⠀
            ⠀⠀⠀⣿⠀⠀⠘⣿⣿⣷⡏⠀⠀⢸⣿⣿⡇⠀⠀⠀⢀⣤⡶⠋⣿⣿⡇⠀⠀⢸⣿⣿⠀⠀ ⠀⣿⣿⡇⠀ ⠀⣿⣿⡇⣰⠃⣿⣿⡇⠀⠀ ⠈⠛⣿⣷⡦⢾⣿⣿⠀⠀⠀⠀⠀⠀ 
        ⠀⠀⠀⠀⠀⣿⠀⠀⠀⠸⣿⡟⠀⠀⠀⢸⣿⣿⡇⠀ ⠀⢰⣿⣿⡀⢀⣿⣿⡇⠀ ⠀⢸⣿⣿⠀⠀ ⢠⣿⣿⠇⠀⠀⣿⣿⡿⠁⠀⣿⣿⡇⠀   ⠀⣼⣿⡿⠀⣸⣿⣿⠀⠀⠀⠀⠀⠀ 
        ⠀⠀⠠⠴⠿⠦⠄⠀⠀⠹⠁⠀⠀⠤⠾⠿⠿⠷⠤⠄ ⠈⠻⠿⠛⠉⠙⠿⠟⠁⠀⢸⣿⣿⠓⠶⠾⠟⠃⠀  ⠴⠿⠿⠷⠄⠠⠿⠿⠷⠄ ⠠⠴⠿⠿⠁⠠⠿⠿⠿⠄⠀⠀⠀⠀⠀ 
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀   ⠀⢸⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀         
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠠⠼⠿⠿⠤⠄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀           
        ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣀⣤⣤⡴⠶⠶⠶⠚⠛⠛⠛⠛⠛⠛⠛⠛⠛⠛⠷⠶⠶⢶⣤⣤⣄⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀  ⠀⢀⣠⡶⠟⠋⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠙⠻⢷⣤⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⡿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠻⣶⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣰⡿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣦⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣾⠟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⢿⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣾⠏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢿⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⣠⣶⣿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢿⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⣠⡾⢛⣿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢦⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⣠⣾⠋⠀⣼⠏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠀⠀⠀⠀⠀⠀⠀⠘⣿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢧⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢹⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⣼⠟⠁⠀⢰⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣇⠀⠀⠀⠈⣧⠀⠀⢹⡽⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣷⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⢀⣾⠏⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⡆⠀⠀⠀⢹⣆⠀⠀⢳⡘⣧⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⣾⠇⠀⠀⠀⠀⠀⠀⠀⠀⢀⠀⢸⠀⠘⡄⠀⢀⠀⠀⠀⠀⠸⣿⣆⠀⠀⠀⢿⣆⠀⠈⢷⡈⢿⣄⠀⠀⠀⠀⠀⠀⡀⠀⠀⠀⠀⠀⠀⠀⢹⣇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⢸⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡄⢸⡄⠀⣿⡀⠘⡆⠀⠀⠀⠀⢻⣿⣦⠀⢀⣸⣿⢷⡶⠚⢿⡄⠻⣷⣄⠀⠀⠀⠀⣷⠀⠀⠀⠀⠀⠀⠀⠀⣿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⣿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣇⢸⡇⠀⣿⢷⡀⢿⡄⠀⠀⠀⠈⣿⡙⢷⣍⠀⠘⣧⠻⣦⡈⢻⣆⠈⠻⣧⣄⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⢸⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⢸⣿⠀⢸⠈⣧⡘⣿⣦⠀⠀⠀⠘⣧⠈⠻⢷⣄⠈⢷⡈⠛⣷⣿⣷⣤⣬⣿⣷⣄⣹⡇⠀⠀⠀⠀⠀⠀⠀⠀⣿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⣿⡀⠀⠀⠀⣴⠀⠀⠀⠀⠀⠀⢹⣾⡟⣧⠻⡟⠛⢷⡸⣿⣷⣄⢀⡀⠹⣧⡀⠀⢙⣻⣶⣿⣿⣿⣿⣿⣿⣿⣿⣿⡿⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⢸⣇⠀⣰⠀⢿⡄⠀⠀⠀⠀⠀⠈⣿⣷⠹⡆⢷⠀⠈⢻⣿⣿⡻⣧⣿⣦⡘⣷⡀⣾⡿⠟⠉⣿⣿⣿⣿⣿⣿⣿⣿⠇⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⢿⡄⢻⣇⠸⣧⠀⢠⡄⠀⠀⠀⠸⣿⡄⠹⣼⡆⠀⠀⠙⢿⣿⣌⠻⢿⣿⣮⣿⣏⠀⠀⠀⢿⣿⣿⣿⣿⣿⣿⡟⠀⣿⡇⠀⡆⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠈⢿⣼⣿⣆⢿⡆⠈⣿⡄⠀⠀⠀⣻⣿⣿⣿⣿⣦⡀⠀⠀⠉⠻⢧⡄⠙⠻⠯⠛⠃⠀⠀⠸⣯⠛⠿⠟⢉⣿⠁⢀⣿⠁⢀⡇⠀⠀⠀⠀⠀⠀⣿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠈⠻⣿⡿⣿⣿⡄⢹⣿⡄⠀⠀⠈⢹⣇⠀⣿⣿⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⠷⠶⠲⠛⠁⠀⢸⡿⠀⣸⡇⠀⠀⠀⠀⠀⢸⡿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠘⠿⡌⠻⢿⡄⢿⡿⣆⠀⠀⠀⣿⡄⢿⣿⣿⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣾⡇⢠⣿⡇⠀⠀⠀⠀⢀⣿⠇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠈⢻⣮⣿⡙⢷⣄⠀⢹⡄⠘⣇⣹⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⡿⢀⣿⢻⡇⠀⣠⠀⠀⣼⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⢿⣿⡄⠉⠻⢾⡇⠀⠛⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⣣⡿⠃⣸⡇⢀⡏⠀⣰⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠻⡆⠀⠈⣧⠀⠀⠀⢦⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⣿⠟⠁⠀⣿⠁⣼⠁⣰⡿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⠀⠀⢻⡄⠀⠀⠀⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⡿⠟⠁⠀⠀⢀⣿⣸⡏⣰⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⡟⠀⠀⠀⠻⣦⡀⠀⠀⠀⠀⠀⠀⠀⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⣿⣿⣼⠏⠀⠀⠀⠀⢀⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⠃⠀⠀⠀⠀⠙⢿⣦⡀⠀⠀⠀⠀⠈⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⣿⡿⠃⠀⠀⠀⠀⢀⣾⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⡟⠀⠀⠀⠀⠀⠀⠀⠙⢿⣦⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣾⣿⠟⠁⠀⠀⠀⠀⢠⣾⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣦⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣤⣶⣿⠟⠁⠀⠀⠀⠀⠀⠀⣰⣿⠟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⡏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡄⠈⢿⣆⠀⠀⠀⠀⢀⣀⣠⣤⡶⠿⠛⢩⣾⠋⠀⠀⠀⠀⠀⠀⢀⣾⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⢀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⠇⠀⠀⠙⠛⠛⠛⠛⠛⠉⠙⢿⡄⠀⣰⡟⠁⠀⠀⠀⠀⠀⢀⣴⣟⣁⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣸⣏⣿⠀⠀⠀⢠⠀⠀⠀⠀⠀⠀⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⣾⠏⠀⠀⠀⠀⠀⢀⣴⠟⠋⠉⠉⠉⠛⠻⢶⣤⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⠀⠀⠀⡇⠀⠀⠀⠀⠀⠀⢻⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡿⠃⠀⠀⠀⠀⢀⣴⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⣿⣿⠀⠀⢸⣇⠀⠀⠀⠀⠀⠀⠸⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⣰⡟⠁⠀⠀⠀⢀⣴⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⣷⡄⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⣧⠀⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣿⡿⢿⡄⠀⢸⣿⡄⠀⠀⠀⠀⠀⠀⢻⣆⠀⠀⠀⠀⠀⠀⠀⣰⡟⠀⠀⠀⠀⣰⡿⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢿⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀⢿⣇⠀⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣇⠘⣷⠀⠸⣇⢿⡄⠀⠀⠀⠀⠀⠀⢻⣶⣄⠀⠀⠀⠀⣰⡟⠀⠀⠀⠀⣼⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢿⣆⠀⠀⠀⠀⠀⠀⠀⠀⠘⣿⡆⠀⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⣿⠀⠙⣷⡀⢻⡌⢿⣆⠀⠀⠀⠀⠀⠀⠹⣿⣧⠀⠀⢠⡟⠀⠀⠀⠀⣸⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢿⡄⠀⠀⠀⠀⠀⠀⠀⠀⠘⣿⡄⠀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢿⡄⠀⠈⠻⣦⡻⣦⣻⣧⡀⠀⠀⠀⠀⠀⠹⣿⠀⠀⣾⠁⠀⠀⠀⢠⣿⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠹⣿⡀⠀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠃⠀⠀⠀⠈⠻⢿⣿⣿⣷⡄⠀⠀⠀⠀⠀⠹⡇⢰⡟⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠹⣷⡀⠀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠙⣿⡀⠀⠀⠀⠀⠀⠃⢸⡇⠀⠀⠀⠀⢸⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠹⣷⡀⠀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡇⠀⠀⠀⠀⠀⣴⠟⣧⠀⠀⠀⠀⠈⣿⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⣷⡀⠀
                                                      ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⠇⠀⠀⠀⣠⡾⠋⠀⢻⣆⠀⠀⠀⠀⠹⣷⡀⠀⠀⠀⠀⠀⠀   ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⢿⡄
                                                      
                                                      
                                                                    Создана Акулининым Андреем и Киселевай Александрой, РХТУ им. Д.И., группа Кс-26
                                                                              Курсова работа по дисциплине "Технологии программирования"
                                                                                                    Москва, 2024
⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀     ⠀⠀⠀⠀
Ваша Мария умеет:
* производить поисковый запрос в поисковой системе Google
  (а также, иногда, открывать сами результаты данного запроса);
* производить поисковый запрос видео в YouTube;
* выполнять поиск определения в Wikipedia c дальнейшим прочтением первых предложений;
* искать человека по имени и фамилии в соцсетях ВКонтакте;
* распознавать и синтезировать речь в offline-моде (без доступа к Интернету);
* "подбрасывать монетку";
* воспроизводить случайное приветствие;
* воспроизводить случайное прощание с последующим завершением работы программы;
* менять настройки языка распознавания и синтеза речи;

Голосовой ассистент использует для синтеза речи встроенные в операционную систему Windows 10 возможности
(т.е. голоса зависят от операционной системы). Для этого используется библиотека pyttsx3

Для корректной работы системы распознавания речи в сочетании с библиотекой SpeechRecognition
используется библиотека PyAudio для получения звука с микрофона.

------------------------------------------------------------------------------------------------------------------------
Как работает Мария
Мария слушает вас, и первое слово распознает как ключевое. По нему она определяет команду к исполнению.
Всё остальное она определяет как запрос. Пожалуйста, при использовании и вы помогайте Марии! Формулируйте
свой запрос, учитывая данную конструкцию. Спасибо.

    Ключевые слова (называются первыми) и соответствующая им команда:
  *  "hello", "hi", "morning", "привет", "здравствуй", "здравствуйте", "хай", "доброе" -> проигрывается приветствие
  *  "bye", "goodbye", "quit", "exit", "stop", "пока", "бай", "выход", "выйди", "выйти", "стоп" ->
                                                                                                проигрывается прощание
  *  "search", "google", "find", "найди", "ищи", "узнай", "расскажи", "что" -> ищется запрос в гугле
  *  "video", "youtube", "watch", "видео", "ютуб", "видосик" -> ищется запрос на ютубе
  *  "wikipedia", "definition", "about", "определение", "википедия", "значение") -> ищется запрос на википедии,
  *  "translate", "interpretation", "translation", "перевод", "перевести", "переведи") -> переводится запрос в
                                                                                        яндекс переводчике (в браузере)
  *  "language", "язык", "изменить", "измени", "change") -> изменяется язык (с русского на английский и наоборот)
  *  "weather", "forecast", "погода", "прогноз") -> прогноз погоды (в браузере) по запросу
                                                                        (предполагается, что запрос - название города)
  *  "vk", "person", "run", "пробей", "контакт", "вконтакте", "вк", "соц" -> открывается Вконтакте в браузере и
                                    ищется человек (запрос выглядит как фамилия и имя человека, которого нудно найти)
  *  "toss", "coin", "монета", "подбрось", "решка", "орёл" -> "нарандоме" называется орел или решка
  *  "угар", "чума", "дэмн", "хайп", "эщкере", "круто", "прикольно" -> просто забавно отвечает на стандартные фразы
