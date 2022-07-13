1. make a directory in apollo/modules/map/data by the name of the map.
2. copy to it base_map.xml
3. run in apollo docker container:
	* dir_name=modules/map/data/demo # example map directory
	./scripts/generate_routing_topo_graph.sh --map_dir ${dir_name}
        
        * dir_name=modules/map/data/demo # example map directory
        bazel-bin/modules/map/tools/sim_map_generator --map_dir=${dir_name} --output_dir=${dir_name}

