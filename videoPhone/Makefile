MXMLC46:=/Applications/Adobe\ Flash\ Builder\ 4.5/sdks/4.6.0/bin/mxmlc

all: bin-release/VideoPhone11.swf

clean:
	rm -f bin-release/VideoPhone.swf bin-release/VideoPhone45.swf bin-release/VideoPhone11.swf

bin-release/VideoPhone11.swf:
	${MXMLC46} -output $@ -compiler.debug=false \
	-define=CONFIG::sdk4,true -define=CONFIG::player11,true \
	-swf-version=13 -target-player 11.1 \
	-locale=en_US -source-path=locale/{locale} \
	-static-link-runtime-shared-libraries=true -source-path src -- src/VideoPhone.mxml
