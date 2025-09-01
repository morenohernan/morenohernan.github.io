---
title: ""
reading_time: false
share: false
---

<!-- Contenedor principal: columna izquierda (logo) + derecha (form) -->
<div style="
  display:grid;
  grid-template-columns: minmax(280px,360px) minmax(640px,1fr);
  gap: 2.5rem;
  align-items: start;
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem 1rem;
">

  <!-- Columna izquierda: LOGO alineado a la izquierda + texto debajo -->
  <div style="align-self:start; display:flex; flex-direction:column; justify-content:flex-start; width:100%;">
    <img src="/media/sistecma.svg" alt="Sistecma" style="width:220px; max-width:100%; margin-bottom:1rem;">
    <p style="font-size:0.95rem; line-height:1.5; color:#374151;">
      Consulta por nuestros servicios y obtén ofertas y beneficios para individuales y grupales.
    </p>
  </div>

  <!-- Columna derecha: FORM ocupa todo el ancho disponible -->
  <div style="width:100%; max-width:820px;">
    <form action="https://formsubmit.co/info@sistecma.io" method="POST" style="margin-bottom: 1rem;">

  <div style="margin-bottom: 1rem;">
        <label for="name" style="display:block; margin-bottom:0.25rem; font-weight:600;">Nombre</label>
        <input type="text" id="name" name="name" required
               oninvalid="this.setCustomValidity('Por favor, ingresa tu nombre')"
               oninput="this.setCustomValidity('')"
               style="width:100%; padding:0.5rem; border:1px solid #d1d5db; border-radius:0.5rem;">
      </div>

   <div style="margin-bottom: 1rem;">
        <label for="email" style="display:block; margin-bottom:0.25rem; font-weight:600;">Email</label>
        <input type="email" id="email" name="_replyto" required
               pattern="[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
               title="Por favor ingresa un email válido (ejemplo: usuario@dominio.com)"
               style="width:100%; padding:0.5rem; border:1px solid #d1d5db; border-radius:0.5rem;">
      </div>

   <div style="margin-bottom: 1rem;">
        <label for="phone" style="display:block; margin-bottom:0.25rem; font-weight:600;">Teléfono</label>
        <input type="tel" id="phone" name="phone"
               style="width:100%; padding:0.5rem; border:1px solid #d1d5db; border-radius:0.5rem;">
      </div>

   <div style="margin-bottom: 1rem;">
        <label for="message" style="display:block; margin-bottom:0.25rem; font-weight:600;">Mensaje</label>
        <textarea id="message" name="message" rows="5" required maxlength="200"
                  oninvalid="this.setCustomValidity('Por favor, deja un mensaje')"
                  oninput="updateCharCount(this)"
                  style="width:100%; padding:0.5rem; border:1px solid #d1d5db; border-radius:0.5rem;"></textarea>
        <div id="charCount" style="text-align:right; font-size:12px; color:#666; margin-top:5px;">0/200</div>
      </div>

   <input type="hidden" name="_next" value="https://sistecma.io/thanks">
      <input type="hidden" name="_subject" value="Nuevo mensaje de contacto">

   <button
        style="padding:0.75rem 1rem; border-radius:0.5rem; font-weight:600;
               background-color:#2563eb; color:white; border:none; cursor:pointer; width:100%;">
        Enviar
      </button>
    </form>
  </div>
</div>

<!-- Bloque descriptivo a ancho completo -->
<div style="max-width: 1280px; margin: 2rem auto; text-align:left; font-size:1.125rem; line-height:1.75; padding:0 1rem;">
  <p style="margin:0;">
    <strong>¿Quiénes somos?</strong> <br/>¡En <span style="color:#ff0404; font-weight:600;">Sistecma</span>, nos dedicamos a convertir tu negocio en un <em>"AI Powered Business"</em>. 
    Nuestro equipo de expertos te ayudará a <strong>automatizar</strong> / <strong>integrar</strong> / <strong>escalar</strong> con la IA para generar mucho más valor. 
    Creemos que la explotación de sus capacidades es un vector para impulsar el crecimiento y la eficiencia. 
    ¡Únete a nosotros en este emocionante viaje a la transformación empresarial e individual con entidades artificiales! 
    <span style="display:block; margin-top:0.75rem;">👉 Contáctanos hoy mismo.</span>
  </p>
</div>

<style>
/* Tablet: dos columnas, más equilibradas */
@media (max-width: 1024px) {
  div[style*="grid-template-columns"] {
    grid-template-columns: minmax(240px,320px) minmax(480px,1fr) !important;
    gap: 2rem !important;
  }
}

/* Móvil: logo arriba, form abajo */
@media (max-width: 768px) {
  div[style*="grid-template-columns"] {
    grid-template-columns: 1fr !important;
    gap: 1.25rem !important;
  }
  /* en móvil, el logo y texto se centran */
  div[style*="justify-content:flex-start"] { justify-content:center !important; text-align:center !important; }
}
</style>

<script>
function updateCharCount(textarea) {
  const charCount = document.getElementById('charCount');
  const n = textarea.value.length;
  charCount.textContent = `${n}/200`;
  charCount.style.color = (n > 180) ? '#dc2626' : '#666';
  textarea.setCustomValidity('');
}
</script>
