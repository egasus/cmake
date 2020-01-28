### single
build.single:
	@if [ -d "single/build" ]; then rm -rf single/build; fi
	@mkdir single/build && \
	 cd single/build && \
	 cmake .. && \
	 make
	@./single/build/hello

build.install:
	@if [ -d "install/build" ]; then rm -rf install/build; fi
	@mkdir install/build && \
	 cd install/build && \
	 cmake .. -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=`pwd`/install && \
	 cmake --build . --config Release --target install
	@./install/build/bin/hello
	
build.lib:
	@if [ -d "lib/build" ]; then rm -rf lib/build; fi
	@mkdir lib/build && \
	 cd lib/build && \
	 cmake .. && \
	 make
	@cd lib/build &&./sayhello

build.complex:
	@if [ -d "complex/build" ]; then rm -rf complex/build; fi
	@mkdir complex/build && \
	 cd complex/build && \
	 cmake .. && \
	 make
	@cd complex/build &&./sayhello

build.multiple:
	@if [ -d "multiple/build" ]; then rm -rf multiple/build; fi
	@mkdir multiple/build && \
	 cd multiple/build && \
	 cmake .. && \
	 make
	@./multiple/build/useHello