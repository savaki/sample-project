desc 'create some artifacts'
task :build do
	run_command <<EOF
mkdir -p target/samples
echo "the time has come the walrus said" > target/samples/sample1.txt 
echo "to speak of many things" > target/samples/sample2.txt
EOF
end

def run_command(command)
	puts command
	system(command) || raise("unable to execute command => #{command}")
end

