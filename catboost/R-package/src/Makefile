unexport YA_BUILD_RESULTS_REPORT

.PHONY : libcatboostr.so

THIS_DIR := $(dir $(abspath $(lastword $(MAKEFILE_LIST))))

libcatboostr.so:
	@if [ "${TRAVIS}" == "true" ]; then         \
		~/build/${TRAVIS_REPO_SLUG}/ya make -r; \
	else                                        \
		../../../ya make -r;                    \
	fi
