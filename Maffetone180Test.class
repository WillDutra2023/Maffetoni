/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */

import maffetone180.Maffetone180;
import org.junit.After;
import org.junit.AfterClass;
import org.junit.Before;
import org.junit.BeforeClass;
import org.junit.Test;
import static org.junit.Assert.*;

/**
 *
 * @author patati
 */
public class Maffetone180Test {
    
    Maffetone180 maffetone;
    
    public Maffetone180Test() {
    }
    
    @BeforeClass
    public static void setUpClass() {
    }
    
    @AfterClass
    public static void tearDownClass() {
    }
    
    @Before
    public void setUp() {
        maffetone = new Maffetone180();
    }
    
    @After
    public void tearDown() {
    }

    @Test
    public void semAlteracoes(){
             
        assertEquals(150, maffetone.calcularMaxCardiaco(30,false,false,false,false));
        assertEquals(140, maffetone.calcularMinCardiaco(maffetone.calcularMaxCardiaco(30,false,false,false,false)));


    }
    
    @Test
    public void convalescente(){
             
        assertEquals(140, maffetone.calcularMaxCardiaco(30,true,false,false,false));
        assertEquals(130, maffetone.calcularMinCardiaco(maffetone.calcularMaxCardiaco(30,true,false,false,false)));


    }
    
    @Test
    public void sedentario(){
             
        assertEquals(145, maffetone.calcularMaxCardiaco(30,false,true,false,false));
        assertEquals(135, maffetone.calcularMinCardiaco(maffetone.calcularMaxCardiaco(30,false,true,false,false)));
         

    }
    
    @Test
    public void ativoConstipado(){
             
        assertEquals(150, maffetone.calcularMaxCardiaco(30,false,false,true,false));
        assertEquals(140, maffetone.calcularMinCardiaco(maffetone.calcularMaxCardiaco(30,false,false,true,false)));
         

    }
    
    @Test
    public void ativo(){
             
        assertEquals(155, maffetone.calcularMaxCardiaco(30,false,false,false,true));
        assertEquals(145, maffetone.calcularMinCardiaco(maffetone.calcularMaxCardiaco(30,false,false,false,true)));


    }

}
