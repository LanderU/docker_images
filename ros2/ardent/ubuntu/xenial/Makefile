all: help

help:
	@echo ""
	@echo "-- Help Menu"
	@echo ""
	@echo "   1. make build            - build all images"
	@echo "   2. make pull             - pull all images"
	@echo "   3. make clean            - remove all images"
	@echo ""

build:
	@docker build --tag=osrf/ros2:ardent-ros-core			ros-core/.
	@docker build --tag=osrf/ros2:ardent-ros-base			ros-base/.
	@docker build --tag=osrf/ros2:ardent-desktop			desktop/.
	@docker build --tag=osrf/ros2:ardent-ros1-bridge			ros1-bridge/.

pull:
	@docker pull osrf/ros2:ardent-ros-core
	@docker pull osrf/ros2:ardent-ros-base
	@docker pull osrf/ros2:ardent-desktop
	@docker pull osrf/ros2:ardent-ros1-bridge

clean:
	@docker rmi -f osrf/ros2:ardent-ros-core
	@docker rmi -f osrf/ros2:ardent-ros-base
	@docker rmi -f osrf/ros2:ardent-desktop
	@docker rmi -f osrf/ros2:ardent-ros1-bridge
