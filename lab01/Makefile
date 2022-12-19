./bin/Linux/main_original: src/main_original.cpp src/glad.c include/utils.h
	mkdir -p bin/Linux
	g++ -std=c++11 -Wall -Wno-unused-function -g -I ./include/ -o ./bin/Linux/main_original src/glad.c src/main_original.cpp ./lib-linux/libglfw3.a -lrt -lm -ldl -lX11 -lpthread -lXrandr -lXinerama -lXxf86vm -lXcursor

./bin/Linux/main_fan: src/main_fan.cpp src/glad.c include/utils.h
	mkdir -p bin/Linux
	g++ -std=c++11 -Wall -Wno-unused-function -g -I ./include/ -o ./bin/Linux/main_fan src/glad.c src/main_fan.cpp ./lib-linux/libglfw3.a -lrt -lm -ldl -lX11 -lpthread -lXrandr -lXinerama -lXxf86vm -lXcursor

./bin/Linux/main_strip: src/main_strip.cpp src/glad.c include/utils.h
	mkdir -p bin/Linux
	g++ -std=c++11 -Wall -Wno-unused-function -g -I ./include/ -o ./bin/Linux/main_strip src/glad.c src/main_strip.cpp ./lib-linux/libglfw3.a -lrt -lm -ldl -lX11 -lpthread -lXrandr -lXinerama -lXxf86vm -lXcursor

./bin/Linux/main_counter: src/main_counter.cpp src/glad.c include/utils.h
	mkdir -p bin/Linux
	g++ -std=c++11 -Wall -Wno-unused-function -g -I ./include/ -o ./bin/Linux/main_counter src/glad.c src/main_counter.cpp ./lib-linux/libglfw3.a -lrt -lm -ldl -lX11 -lpthread -lXrandr -lXinerama -lXxf86vm -lXcursor



.PHONY: clean run
clean:
	rm -f bin/Linux/main_original
		rm -f bin/Linux/main_strip
	rm -f bin/Linux/main_fan

original: ./bin/Linux/main_original
	cd bin/Linux && ./main_original

fan: ./bin/Linux/main_fan
	cd bin/Linux && ./main_fan

strip: ./bin/Linux/main_strip
	cd bin/Linux && ./main_strip

counter: ./bin/Linux/main_counter
	cd bin/Linux && ./main_counter
