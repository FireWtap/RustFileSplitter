# RustFileSplitter
Uses rust to split a file in several chunk by given fixed size. Then recomposes it as needed
Very simple implementation.



## Installation
Simply add the library to your Cargo.toml as such:
`[dependencies]`

`rust_file_splitting_utils = { git = "https://github.com/FireWtap/RustFileSplitter", branch = "main" }`


## Split
`rust_file_splitting_utils::file_splitter::split(FILENAME <String>, Size in Byte <Usize>, Output Dir <String>);`

Returns a vector containing the path of all the chunks created. 
The chunks are given in order, this is important since they will be used in such order to get merged back.


## Merge

`rust_file_splitting_utils::file_merger::merge(Output Name <String>, Output Dir <String>, Vector of all the parts path <vec<String>>);`


Feel free to push a new update if you have any improvement on this code.
Keep in mind I'm a beginner in Rust.


