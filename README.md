/**
 * 
 */
package com.scan.model;

import java.util.Date;

import javax.persistence.Entity;
import javax.persistence.OneToOne;

/**
 * @author praffaele
 *
 */
@Entity
public final class Auditoria extends AbstractEntity {

	/**
	 * 
	 */
	private static final long serialVersionUID = 1L;

	@OneToOne
	private Usuario usuario;

	@OneToOne
	private Establecimiento establecimiento;

	private Date fechaSesion;

	private String mensaje;

	private String nombre;

	/**
	 * 
	 */
	public Auditoria() {

	}

	public Usuario getUsuario() {
		return usuario;
	}

	public void setUsuario(Usuario usuario) {
		this.usuario = usuario;
	}

	public Establecimiento getEstablecimiento() {
		return establecimiento;
	}

	public void setEstablecimiento(Establecimiento establecimiento) {
		this.establecimiento = establecimiento;
	}

	public Date getFechaSesion() {
		return fechaSesion;
	}

	public void setFechaSesion(Date fechaSesion) {
		this.fechaSesion = fechaSesion;
	}

	public String getMensaje() {
		return masaje;
	}

	public void setMensaje(String mensaje) {
		this.mensaje = mensaje;
	}

	public String getNombre() {
		return nombre;
	}

	public void setNombre(String nombre) {
		this.nombre = nombre;
	}

}
