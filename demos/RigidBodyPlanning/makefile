CC = g++
CFLAGS = -g -Wall -std=c++14 -std=c++11 -I/usr/local/include/ompl-1.5 -I/usr/include/eigen3
LDFLAGS=-L/usr/local/lib -lompl -lompl_app_base -lompl_app /usr/lib/x86_64-linux-gnu/libboost_serialization.so /usr/lib/x86_64-linux-gnu/libboost_filesystem.so /usr/lib/x86_64-linux-gnu/libboost_system.so -lpthread /usr/lib/x86_64-linux-gnu/libOpenGL.so /usr/lib/x86_64-linux-gnu/libGLX.so /usr/lib/x86_64-linux-gnu/libGLU.so -lode -lfcl
#LDFLAGS=
TARGET = RigidBodyPlanning

all: $(TARGET)
$(TARGET): $(TARGET).cpp
	$(CC) $(CFLAGS) -o $(TARGET) $(TARGET).cpp $(LDFLAGS)
clean:
	$(RM) $(TARGET)
