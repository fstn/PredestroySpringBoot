# PredestroySpringBoot
add predestroy in springboot

 //Add shutdown hook in order to call @PreDestroy annotation
        Runtime.getRuntime().addShutdownHook(new Thread()
        {
            public void run() {
                applicationContext.close();
            }
        });
