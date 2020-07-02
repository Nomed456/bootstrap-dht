cc_binary(
    name = "bootstrap-dht",
    srcs = [
        "main.cpp",
    ],
    deps = [
        ":bencoder",
        "@boost//:uuid",
        "@boost//:asio",
        "@boost//:system",
        "@boost//:crc",
        "@boost//:circular_buffer"
    ],
)

cc_library(
    name = "bencoder",
    srcs = [
        "bdecode.cpp",
        "bdecode.hpp",
        "bencode.hpp",
    ],
    hdrs = [ "bdecode.hpp" ],
    deps = [ ":utils" ],
)

cc_library(
    name = "utils",
    srcs = [
        "span.hpp",
        "node_buffer.hpp",
        "ip_set.hpp",
        "ip_set.cpp",
        "city.h",
        "city.cc",
        "mapped_file.hpp",
        "ping_queue.hpp",
        "config.h",
    ],
)