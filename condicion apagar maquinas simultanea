public void apagarpc() throws IOException{
	   String shutdownCommand;
	    String operatingSystem = System.getProperty("name");

	    if ("Linux".equals(operatingSystem) || "Mac OS X".equals(operatingSystem)) {
	        shutdownCommand = "shutdown -h now";
	    }
	    else if (operatingSystem.contains("Windows")) {
	        shutdownCommand = "shutdown.exe -s -t 0";
	    }
	    else {
	        throw new RuntimeException("Sistema operativo no compatible.");
	    }

	    Runtime.getRuntime().exec(shutdownCommand);
	    System.exit(0);
	   }
