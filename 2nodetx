from test_framework.test_framework import BitcoinTestFramework

Class ExampleTest(BitcoinTestFramework):
	
	# create two nodes
	def set_test_params(self):
		self.setup_clean_chain = True
		self.num_nodes = 2

	# start up nodes
	def setup_network(self):
		self.setup_nodes( )
		self.connect_nodes(0,1)
	
	# node 1 mints block
	def custom_method(self):
	block = create_block(self.tip, self.block_time)
		block.solve( )

	# sends block to node 2
	def run_test(self):
		block_message = msg_block(block)
		peer_messaging.send_message(block_message)

	# logs Node 2 received the block						
		self.nodes.sync_all() 
		getdata_request = msg_getdata()

if __name__ == '__main__':
    ExampleTest().main()
