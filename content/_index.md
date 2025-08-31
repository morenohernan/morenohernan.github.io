---
title: 'Home'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: hero
    content:
      title: Transforma tu Negocio con la IA
      text:  "La mejor manera de predecir el futuro es crearlo -- Peter Drucker"
      # primary_action:
      #   text: "info\\@sistecma.io"
      #   url: https://hugoblox.com/templates/
      #   icon: user
      # secondary_action:
      #   text: "Schedule an appoinment "
      #   url: https://docs.hugoblox.com
      # announcement:
      #   text: "Announcing the release of version 1."
      #   link:
      #     text: "Read more"
      #     url: "/blog/"
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: "dark"
      background:
        color: "navy"
        image:
          # Add your image background to `assets/media/`.
          filename: neural-network.svg
          filters:
            brightness: 0.5
          size: cover
          position: center
          parallax: false
  - block: stats
    content:
      items:
        - statistic: "+20%"
          description: |
            Ahorro en costos operativos
        - statistic: "+15%"
          description: |
            Incremento en ventas por automatización
        - statistic: "+30%"
          description: |
            Velocidad de respuesta al mercado
    design:
      # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-900"
      # Reduce spacing
      spacing:
        padding: ["1rem", 0, "1rem", 0]
  - block: features
    id: solutions
    content:
      title: Inteligencia Estratégica #Soluciones
      text: Transforma tu operación con procesos inteligentes, y decisiones más rápidas. Haz de cada proceso una ventaja competitiva #"Simples, prácticas y a tu alcance"
      items:
        - name: Automatiza
          icon: arrow-path
          description: Lo que consume tiempo y gana foco en lo que genera valor.
                       Procesos más claros. 
                       Tiempos más cortos. 
                       Menos errores.
        - name: Integra
          icon: link
          description: "Tu negocio a la IA: cada interacción, cada dato y cada proceso se convierte en inteligencia accionable y convierte tus procesos en motores de crecimiento. Tus sistemas no solo ejecutan tareas, sino que anticipan necesidades, aceleran decisiones y te dan ventaja frente a tu competencia"
        - name: Escala
          icon: arrows-pointing-out
          description: Tu conocimiento, amplificado con IA. 
                       Atención al cliente que responde sola.
                       Operaciones que no olvidan.
                       Ventas que no se detienen.
                       Equipos que aprenden más rápido  
        # - name: No-Code
        #   icon: code-bracket
        #   description: Edit and design your site just using rich text (Markdown) and configurable YAML parameters.
        # - name: Highly Rated
        #   icon: star
        #   description: Rated 5-stars by the community.
        # - name: Swappable Blocks
        #   icon: rectangle-group
        #   description: Build your pages with blocks - no coding required!
  - block: cta-image-paragraph
    id: solutions
    content:
      items:
        - title: Tu negocio evoluciona, tu visión también.
          text: "Hoy las empresas que crecen no solo se digitalizan: automatizan, integran, aprenden y escalan. Lo que antes tomaba semanas, ahora se resuelve en horas. Lo que parecía complejo, ahora fluye."
          feature_icon: check
          features:
            - "Automatiza lo repetitivo."
            - "Integra tus sistemas y procesos con inteligencia."
            - "Escala y explota el conocimiento, con datos que generan valor real."
            - "Evolucionar con IA no es solo mejorar procesos: es abrir la puerta a nuevas formas de crecer, competir y liderar."
          # Upload image to `assets/media/` and reference the filename here
          image: business-evolution.png
          button:
            text: Estoy interesado
            url: /#contact
        - title: "Así transformamos tu empresa"
          text:  Conoce nuestro enfoque
          feature_icon: bolt
          features:
            - "La Ejecución Durable (DEx) actúa como la capa invisible que conecta la IA con los procesos de negocio. A diferencia de las automatizaciones tradicionales, que suelen ser frágiles y difíciles de mantener, este enfoque permite que cualquier flujo de trabajo se ejecute de manera confiable sin importar si dura segundos, días, meses, o años, e incluso si hay fallos, interrupciones o reinicios en el sistema."
            - "El Modelo de Contexto (MCP) funciona como un traductor universal que permite que la IA entienda y utilice la información de tu empresa de la misma manera que lo haría un equipo humano. Conecta datos dispersos, documentos y sistemas en un solo lenguaje, lo que facilita que las respuestas y acciones sean siempre relevantes, precisas y alineadas con tu negocio."
            - "El enfoque Multi-Agente transforma a la IA en un equipo de especialistas digitales que colaboran entre sí. Se despliegan agentes con roles claros y capacidades complementarias: uno busca información, otro razona escenarios, otro valida resultados y otro comunica con claridad. Este modelo multiplica la precisión y la eficiencia."
            - "La Generación Aumentada por Recuperación (RAG) permite que la IA responda con contexto real y familiar a tu negocio. En lugar de limitarse a generar texto, se conecta con tus propias bases de conocimiento, documentos o sistemas, y trae información precisa para enriquecer cada respuesta."
          # Upload image to `assets/media/` and reference the filename here
          image: value-proposition.png
          # button:
          #   text: Join Discord
          #   url: https://discord.gg/z8wNYzb
    design:
      # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-900"
      css_class: "dark:bg-gray-900"
  - block: testimonials
    content:
      title: ""
      text: ""
      items:
        - name: "Amelia Moreno"
          role: "Product Director at Mignonette Inc."
          # Upload image to `assets/media/` and reference the filename here
          image: "testimonial-1.jpg"
          text: "¡Genial, Sistecma nos ayudó a incrementar nuestras ventas rápidamente. A los 3 meses de transformar nuestros sistemas a entidades inteligentes ya teníamos resultados tangibles!"
    design:
      spacing:
        # Reduce bottom spacing so the testimonial appears vertically centered between sections
        padding: ["6rem", 0, 0, 0]

  - block: cta-card
    content:
      title: Tu negocio, más ágil. Tus equipos, más efectivos. Tus clientes, más cerca.
      text: Productividad, Velocidad y Valor real.
    design:
      # Primero configurar el card:
      card:
        css_class: "text-white custom-font-size"
        css_style: "background: linear-gradient(rgba(18, 24, 40, 0.3), rgba(18, 24, 40, 0.3)), url('/media/neural-network.svg') !important; background-size: cover !important; background-position: center !important; border-radius: 20px !important; padding: 80px 40px !important; background-color: transparent !important;"
---
